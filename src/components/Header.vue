<template>
  <header class="container primary_color_text fw_600">
    <div class="row_aligned fs_small txt_uppercase">
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
          <li v-for="(link, index) in linksArray" :key="index">
            <a :href="link.url" :class="{brand_color_text: link.current}">{{ link.text }}</a>
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
header {
  height: 100px;

  img {
    height: 75px;
    margin: 15px;
  }
  li {
    display: inline-block;
    margin: 0 10px;
    :hover {
      color: rgb(24, 131, 240);
    }
  }
}
</style>
