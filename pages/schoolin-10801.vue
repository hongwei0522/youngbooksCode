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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n08/1.jpg') },
        { hid: 'description', name: 'description', content: '士林高商「獨享的空間」' },
        { hid: 'og:description' , property: 'og:description' , content: '士林高商「獨享的空間」' },
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
      detail: { img: require('@/assets/img/article/n08/1.jpg'), position: 'v', name: '士林高商', place: 'n', title: '獨享的空間', desc: '花生俠', content: '成功的人往往是獨來獨往的。如果不喜歡和別人坐在一起讀書，這裡是能讓人獨享的好空間。', link: '10801' }
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