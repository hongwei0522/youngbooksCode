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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n08/8.jpg') },
        { hid: 'description', name: 'description', content: '士林高商「夢幻閱讀私角落」' },
        { hid: 'og:description' , property: 'og:description' , content: '士林高商「夢幻閱讀私角落」' },
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
      detail: { img: require('@/assets/img/article/n08/8.jpg'), position: 'v', name: '士林高商', place: 'n', title: '夢幻閱讀私角落', desc: '陳宜均', content: '士林高商圖書館內有張引人注目的椅子，坐在上面不但很舒服，還可以像電影主角般在椅子上優雅的看書。', link: '10808' }
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