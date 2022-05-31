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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n08/9.jpg') },
        { hid: 'description', name: 'description', content: '士林高商「[和室]的地方」' },
        { hid: 'og:description' , property: 'og:description' , content: '士林高商「[和室]的地方」' },
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
      detail: { img: require('@/assets/img/article/n08/9.jpg'), position: 'r', name: '士林高商', place: 'n', title: '[和室]的地方', desc: '花生俠', content: '誰說讀書只能在書桌前，士商圖書館的和室空間，也是合適的讀書環境。', link: '10809' }
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