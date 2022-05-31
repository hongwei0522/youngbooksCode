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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/m01/2.jpg') },
        { hid: 'description', name: 'description', content: '三義高中「落葉歸根」' },
        { hid: 'og:description' , property: 'og:description' , content: '三義高中「落葉歸根」' },
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
      detail: { img: require('@/assets/img/article/m01/2.jpg'), position: 'v', type: 'h', name: '三義高中', place: 'm', title: '落葉歸根', desc: '王玉萱', content: '坐在石椅上看著書，在樹蔭的遮蔽下，有時有花朵和葉片飄落，讓我瞬間變成「為賦新詞強說愁」的少女。', link: '20102' }
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