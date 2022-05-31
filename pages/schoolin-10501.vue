<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '成淵高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n05/1.jpg') },
        { hid: 'description', name: 'description', content: '成淵高中「陽光下的閱讀」' },
        { hid: 'og:description' , property: 'og:description' , content: '成淵高中「陽光下的閱讀」' },
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
      detail: { img: require('@/assets/img/article/n05/1.jpg'), position: 'v', name: '成淵高中', place: 'n', title: '陽光下的閱讀', desc: '云云', content: '位在四樓聯絡走廊，木頭的長椅經常被灑上薄薄的陽光，而我坐在長椅上不僅是閱讀，還能得到正能量。', link: '10501' }
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