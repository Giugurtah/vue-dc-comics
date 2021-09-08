<template>
  <main class="primary_color">
    <div id="content" class="container fw_600 neutral_color_text">
      <header class="main_header d_inline_block brand_color txt_uppercase">Current series</header>
      <section class="card_display row_basic">
        <ComicCard v-for="(comic, index) in DcComics" :key="index" :comic="comic"/>
      </section>
      <div class="button d_inline_block brand_color txt_uppercase fs_small">
        Load more
      </div>
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
    padding-top: 30px;
    position: relative;

    .main_header {
      padding: 10px 20px;
      position: absolute;
      top: 0;
      transform: translateY(-50%);
    }

    .card_display {
      flex-wrap: wrap;
    }

    .button {
      padding: 10px 40px;
      position: relative;
      left: 50%;
      transform: translateX(-50%);

      margin-bottom: 15px;
    }
  }
}
</style>
