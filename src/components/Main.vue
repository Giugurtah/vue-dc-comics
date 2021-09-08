<template>
  <main class="primary_color">
      <div id="content" class="container fw_600 neutral_color_text">
          -- Content goes here --
      </div>
  </main>
</template>

<script>
export default {
  name: 'Main'
}
</script>

<style lang="scss" scoped>
main {
  height: calc(100vh - 500px);
  
  #content {
    line-height: calc(100vh - 500px);
  }
}
</style>
