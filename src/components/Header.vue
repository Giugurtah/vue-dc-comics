<template>
  <header class="container primary_color_text fw_600">
    <div class="row_justified fs_small txt_uppercase">
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
          <li v-for="(link, index) in linksArray" :key="index" :class="{active: link.current}">
            <a :href="link.url" >{{ link.text }}</a>
          </li>
        </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data () {
    return {
      linksArray: [
        {
          text: 'Characters',
          url: '#',
          current: false
        },
        {
          text: 'Comics',
          url: '#',
          current: true
        },
        {
          text: 'Movies',
          url: '#',
          current: false
        },
        {
          text: 'TV',
          url: '#',
          current: false
        },
        {
          text: 'Games',
          url: '#',
          current: false
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false
        },
        {
          text: 'Videos',
          url: '#',
          current: false
        },
        {
          text: 'Fans',
          url: '#',
          current: false
        },
        {
          text: 'News',
          url: '#',
          current: false
        },
        {
          text: 'Shop',
          url: '#',
          current: false
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "@/assets/style/index.scss";
header {
  height: 100px;

  img {
    height: 75px;
    margin: 15px;
  }

  li {
    height: 100%;
    line-height: 100px;

    display: inline-block;
    position: relative;

    margin: 0 10px;
  }
  
  .active {
    color: $brand_color;

    :after {
      content: "";
      width: 100%;
      height: 5px;
      display: inline-block;
      background-color: $brand_color;

      position: absolute;
      bottom: 0;
      left: 0;
      transform: translateY(-100%);
    }
  }
}
</style>
