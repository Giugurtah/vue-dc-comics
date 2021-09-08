<template>
  <footer class="secondary_color">
      <div class="container h-100">
          <div class="row_aligned h-100">
              <div class="button neutral_color_text txt_uppercase fw_600 fs_small">Sign-up now!</div>
              <div class="row align_center">
                  <div class="d_inline_block brand_color_text fw_600 txt_uppercase">Follow us</div>
                  <img v-for="(img, index) in imgArray" :key="index" :src="getUrl(img.link)" :alt="img.name">
              </div>
          </div>
      </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterSocials',
  data () {
    return {
      imgArray: [
        {
          name: 'facebook',
          link: 'footer-facebook.png'
        },
        {
          name: 'twitter',
          link: 'footer-twitter.png'
        },
        {
          name: 'youtube',
          link: 'footer-youtube.png'
        },
        {
          name: 'pinterest',
          link: 'footer-pinterest.png'
        },
        {
          name: 'periscope',
          link: 'footer-periscope.png'
        }
      ]
    }
  },
  methods: {
    getUrl (link) {
      return require('../assets/img/' + link)
    }
  }
}
</script>

<style lang="scss" scoped>
footer {
  height: 100px;
  
  .button {
    border: 2px solid rgb(24, 131, 240);
    padding: 10px;
  }
  img {
    margin-left: 15px;
    height: 30px;
  }
}
</style>
