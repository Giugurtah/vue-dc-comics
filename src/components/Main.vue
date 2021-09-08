<template>
  <main class="primary_color">
    <div id="content" class="container row_basic fw_600 neutral_color_text">
        <ComicCard v-for="(comic, index) in DcComics" :key="index" :comic="comic"/>
    </div>
  </main>
</template>

<script>
import ComicCard from '../components/ComicCard.vue';
import DcComics from '../assets/data/DcComics.js';
export default {
  name: 'Main',
  data() {
    return {
      DcComics,
    }
  },
  components: {
    ComicCard,
  }
}
</script>

<style lang="scss" scoped>
main {
  #content {
    flex-wrap: wrap;
  }

}
</style>
