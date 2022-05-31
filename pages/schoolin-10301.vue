<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '師範大學',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n03/1.jpg') },
        { hid: 'description', name: 'description', content: '師範大學「預言」' },
        { hid: 'og:description' , property: 'og:description' , content: '師範大學「預言」' },
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
      detail: { img: require('@/assets/img/article/n03/1.jpg'), position: 'r', name: '師範大學', place: 'n', title: '預言', desc: '公園', content: '當你抱著書不小心跌倒時，你是否有想過，掉到地上攤開的書，翻到了哪一頁，這是不是個徵兆、或是個預言？', link: '10301' }
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