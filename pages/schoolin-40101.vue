<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '慈大附中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/e01/1.jpg') },
        { hid: 'description', name: 'description', content: '慈大附中「沐浴在晨下」' },
        { hid: 'og:description' , property: 'og:description' , content: '慈大附中「沐浴在晨下」' },
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
      detail: { img: require('@/assets/img/article/e01/1.jpg'), position: 'r', name: '慈大附中', place: 'e', title: '沐浴在晨下', desc: '紀', content: '早晨的陽光輕輕灑在疲憊的身軀上，輕輕灑在慈大校園的角落，沐浴在藍天白雲裡，即使阻礙豎立在眼前，仍然翻開一頁頁書本，翻開我的夢想之路。', link: '40101' }
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