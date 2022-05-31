<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '南投縣復臨國際實驗教育機構',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/m04/1.jpg') },
        { hid: 'description', name: 'description', content: '南投縣復臨國際實驗教育機構「霸氣涼亭」' },
        { hid: 'og:description' , property: 'og:description' , content: '南投縣復臨國際實驗教育機構「霸氣涼亭」' },
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
      detail: { img: require('@/assets/img/article/m04/1.jpg'), position: 'r', type: 'h', name: '南投縣復臨國際實驗教育機構', place: 'm', title: '霸氣涼亭', desc: '怪盜小火龍', content: '學校的涼亭讓我可以霸氣的看書', link: '20401' }
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