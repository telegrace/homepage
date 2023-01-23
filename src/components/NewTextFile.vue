<template>
  <div class="window scale-down new-text-file" style="width:500px;">
    <div class="title-bar">
      <button aria-label="Close" class="close"></button>
      <h1 class="title">New Text File</h1>
      <button aria-label="Resize" disabled class="hidden"></button>
    </div>
    <div class="separator"></div>

    <div class="modeless-dialog">
      Send me a message
      <br/>
      <br />

      <textarea></textarea>
      <br />
      <br />

      <section class="field-row" style="justify-content: flex-end">
        <button class="btn">Cancel</button>
        <button class="btn" style="width:95px;">Send</button>
      </section>
    </div>
  </div>
</template>