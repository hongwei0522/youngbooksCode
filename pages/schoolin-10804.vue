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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n08/4.jpg') },
        { hid: 'description', name: 'description', content: '士林高商「1.9樓」' },
        { hid: 'og:description' , property: 'og:description' , content: '士林高商「1.9樓」' },
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
      detail: { img: require('@/assets/img/article/n08/4.jpg'), position: 'v', name: '士林高商', place: 'n', title: '1.9樓', desc: '小熊餅乾', content: '學校的1.9樓充滿許多樂趣', link: '10804' }
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