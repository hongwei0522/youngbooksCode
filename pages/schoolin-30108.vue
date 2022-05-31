<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '新營高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s01/8.jpg') },
        { hid: 'description', name: 'description', content: '新營高中「圖書館」' },
        { hid: 'og:description' , property: 'og:description' , content: '新營高中「圖書館」' },
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
      detail: { img: require('@/assets/img/article/s01/8.jpg'), position: 'r', type: 'h', name: '新營高中', place: 's', title: '圖書館', desc: 'yu', content: '學校圖書館，不只宣傳人文魅力、文字之美，也貼近自然，寧靜而愜意，為校園裡最自由美好的角落，多添一抹光景。', link: '30108' }
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