<template>
  <div>
    <schoolContain :title="title" :frames="frames" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '長樂國小',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '長樂國小' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n-01_s01_02.jpg') },
        { hid: 'description', name: 'description', content: '基隆長樂國小' },
        { hid: 'og:description' , property: 'og:description' , content: '基隆長樂國小' },
      ],
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
        { img: require('@/assets/img/article/n-01_s01_01.jpeg'), title: '操場也能閱讀？閱讀無限', desc: 'HYC' },
        { img: require('@/assets/img/article/n-01_s01_02.jpg'), title: '閱在花中', desc: '三口' },
        { img: require('@/assets/img/article/n-02_u01_01.jpg'), title: '靜閱', desc: '洗硯' },
        { img: require('@/assets/img/article/n-01_s01_01.jpeg'), title: '操場也能閱讀？閱讀無限', desc: 'HYC' },
        { img: require('@/assets/img/article/n-01_s01_02.jpg'), title: '閱在花中', desc: '三口' },
        { img: require('@/assets/img/article/n-02_u01_01.jpg'), title: '靜閱', desc: '洗硯' },
      ]
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