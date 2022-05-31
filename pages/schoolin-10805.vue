<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '士林高商',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n08/5.jpeg') },
        { hid: 'description', name: 'description', content: '士林高商「舒悅讀」' },
        { hid: 'og:description' , property: 'og:description' , content: '士林高商「舒悅讀」' },
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
      detail: { img: require('@/assets/img/article/n08/5.jpeg'), position: 'r', name: '士林高商', place: 'n', title: '舒悅讀', desc: '鴒鴃', content: '校園中的圖書館，讓人能安心舒適並保持愉悅的心認真閱讀。', link: '10805' }
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