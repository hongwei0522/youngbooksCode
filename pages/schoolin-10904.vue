<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '桃園陽明高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n09/4.jpg') },
        { hid: 'description', name: 'description', content: '桃園陽明高中「青春筆記」' },
        { hid: 'og:description' , property: 'og:description' , content: '桃園陽明高中「青春筆記」' },
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
      detail: { img: require('@/assets/img/article/n09/4.jpg'), position: 'v', name: '桃園陽明高中', place: 'n', title: '青春筆記', desc: 'night', content: '學校的操場旁，不只是同學們打球的地方，旁邊的觀眾台也是我小憩的一方天地。樹下的餘蔭和徐徐吹來的微風，伴隨著此起彼落的歡聲笑語，還有連續不斷的拍球聲。一切成為閱讀的背景音，伴我進入書中世界。', link: '10904' }
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