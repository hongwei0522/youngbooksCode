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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n09/3.jpg') },
        { hid: 'description', name: 'description', content: '桃園陽明高中「門口」' },
        { hid: 'og:description' , property: 'og:description' , content: '桃園陽明高中「門口」' },
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
      detail: { img: require('@/assets/img/article/n09/3.jpg'), position: 'v', name: '桃園陽明高中', place: 'n', title: '門口', desc: '小Z', content: '保持閱讀空間的通風，也帶來了許多額外的生氣。放學後，陽明學生們一個一個走進圖書館，前往自己的閱讀私角落。', link: '10903' }
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