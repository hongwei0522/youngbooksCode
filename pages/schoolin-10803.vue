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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n08/3.jpg') },
        { hid: 'description', name: 'description', content: '士林高商「一介書生」' },
        { hid: 'og:description' , property: 'og:description' , content: '士林高商「一介書生」' },
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
      detail: { img: require('@/assets/img/article/n08/3.jpg'), position: 'v', name: '士林高商', place: 'n', title: '一介書生', desc: '花生俠', content: '書生沒有局限於人類，愛讀書的兔子就躲在士商角落埋頭苦讀呢！', link: '10803' }
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