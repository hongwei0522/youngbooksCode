<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '輔大聖心高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n01/1.jpg') },
        { hid: 'description', name: 'description', content: '輔大聖心高中「閱讀無限制！」' },
        { hid: 'og:description' , property: 'og:description' , content: '輔大聖心高中「閱讀無限制！」' },
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
      // 設定自動抓取
      detail: { img: require('@/assets/img/article/n01/1.jpg'), positon: 'r', name: '輔大聖心高中', place: 'n', title: '閱讀無限制！', desc: 'HYC', content: '學校的操場<br>不只提供學生運動的場地<br>亦可以在此閱讀<br>只要有心<br>不論地點都可以徜徉書海', link: '10101' },
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