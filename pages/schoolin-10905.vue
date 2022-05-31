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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n09/5.jpg') },
        { hid: 'description', name: 'description', content: '桃園陽明高中「寂靜的教室」' },
        { hid: 'og:description' , property: 'og:description' , content: '桃園陽明高中「寂靜的教室」' },
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
      detail: { img: require('@/assets/img/article/n09/5.jpg'), position: 'v', name: '桃園陽明高中', place: 'n', title: '寂靜的教室', desc: '寰', content: '放學後的校園，空蕩蕩安靜的教室與原先熱鬧人聲吵雜迴盪整間教室形成一個極大的對比。', link: '10905' }
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