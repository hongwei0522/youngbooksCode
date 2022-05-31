<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '三義高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/m01/4.jpg') },
        { hid: 'description', name: 'description', content: '三義高中「書海秘境」' },
        { hid: 'og:description' , property: 'og:description' , content: '三義高中「書海秘境」' },
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
      detail: { img: require('@/assets/img/article/m01/4.jpg'), position: 'v', type: 'h', name: '三義高中', place: 'm', title: '書海秘境', desc: '王玉萱', content: '圖書館裡瀰漫著靜謐感，書海中找尋一處角落，寧靜的享受一個人的閱讀時光。', link: '20104' }
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