<script setup lang="ts">
import { ref } from 'vue';

let dragFlag = false
const width = ref("400px")
let intro = "Hi, I'm Grace. I like to make things."
let left = ref<string>(""); 
let top = ref<string>(""); 


const mouseDownHandler =()=>{
  dragFlag=true
}

const mouseUpHandler = ()=>{
  dragFlag=false
}

const mouseMoveHandler = (event) => {
  if (dragFlag) {
    const x = event.clientX;
    const y = event.clientY;
    left.value = x - 400 / 2;
    top.value = y - 100 / 2;
  }
}

</script>


<template>
<div class="standard-dialog center scale-down draggable-box" :style="{width, top:top+'px', left:left + 'px'}" @mousedown="(event)=>mouseDownHandler(event)" @mouseup="mouseUpHandler" @mousemove="(event)=>mouseMoveHandler(event)">
  <h1 class="dialog-text">{{intro}}</h1>
  <p class="dialog-text">Drag me</p>
</div>



</template>
