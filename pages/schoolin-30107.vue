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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s01/7.jpeg') },
        { hid: 'description', name: 'description', content: '新營高中「角落的書牆」' },
        { hid: 'og:description' , property: 'og:description' , content: '新營高中「角落的書牆」' },
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
      detail: { img: require('@/assets/img/article/s01/7.jpeg'), position: 'v', type: 'h', name: '新營高中', place: 's', title: '角落的書牆', desc: '岑', content: '圖書館裡不只能閱讀，還能放鬆心情用心感受書本裡的每一句話。', link: '30107' }
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