<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '三義高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/m01/3.jpg') },
        { hid: 'description', name: 'description', content: '三義高中「大地與我共享」' },
        { hid: 'og:description' , property: 'og:description' , content: '三義高中「大地與我共享」' },
      ],
    }
  },
  layout: 'default',
  components: {
    schoolinContain: require('~/components/schoolin-contain.vue').default,
  },
  props: {
    
  },
  data () {
    return {
      detail: { img: require('@/assets/img/article/m01/3.jpg'), position: 'r', type: 'h', name: '三義高中', place: 'm', title: '大地與我共享', desc: '王玉萱', content: '趴在綠油油的草地，讀著輕小說。湛藍的天空，棉花糖般的雲朵，花草的清香。天馬行空的想像著小說的情節，空氣被粉紅泡泡給填滿了。', link: '20103' }
    }
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