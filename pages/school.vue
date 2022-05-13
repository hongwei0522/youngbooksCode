<template>
  <div>
    <schoolContain :title="title" :frames="frames" />
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
    schoolContain: require('~/components/school-contain.vue').default,
  },
  props: {
    
  },
  data () {
    return {
      title: '長樂國小',
      frames: [
        { img: require('@/assets/img/article/n01/1.jpg'), title: '操場也能閱讀？閱讀無限', desc: 'HYC' },
        { img: require('@/assets/img/article/n01/2.jpg'), title: '閱在花中', desc: '三口' },
        { img: require('@/assets/img/article/n02/1.jpg'), title: '靜閱', desc: '洗硯' },
      ]
    }
  },
  mounted () {
    // 取得網址列參數
    // 取得標題
    // 取得圖片
    // 取得往下一層的連結
  },
  computed: {

  },
  methods: {
    
  },
  watch: {
    
  }
}
</script>

<style lang="scss" scoped>

</style>