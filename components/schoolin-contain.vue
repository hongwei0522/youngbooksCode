<template>
  <div>



    <!-- <div class="school-swiper-social">
      <a :href="`https://www.facebook.com/sharer/sharer.php?u=${fbUrl}&amp;src=sdkpreparse`" target="_blank">
        <img class="school-swiper-icon" src="@/assets/img/icon/fb-share.png" alt="share fb">
      </a>
      <img @click="copy()" class="school-swiper-icon" src="@/assets/img/icon/copy.png" alt="copy link">
      <a :href="`https://social-plugins.line.me/lineit/share?url=${currentUrl}`" target="_blank">
        <img class="school-swiper-icon" src="@/assets/img/icon/line-share.png" alt="share line">
      </a>
    </div> -->
  </div>
</template>

<script>
export default {
  head() {
    return {
    }
  },
  layout: 'default',
  components: {

  },
  props: {
    
  },
  data () {
    return {
      currentUrl: '',
      fbUrl: ''
    }
  },
  mounted () {
    this.currentUrl = window.location.href
    this.fbUrl = window.location.href
    this.fbUrl = this.fbUrl.replaceAll('/', '%2F')
  },
  computed: {

  },
  methods: {
    copy(){
      var domUrl = document.createElement("input");
      domUrl.value = this.currentUrl;
      domUrl.id = "creatDom";
      document.body.appendChild(domUrl);
      domUrl.select(); // 选择对象
      document.execCommand("Copy"); // 执行浏览器复制命令
      let creatDom = document.getElementById("creatDom");
      creatDom.parentNode.removeChild(creatDom);
      this.$message({
          message: '複製成功',
          type: 'success'
      });
    }
  },
  watch: {
    
  }
}
</script>

<style lang="scss" scoped>

</style>