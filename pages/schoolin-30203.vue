<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '三民家商',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s02/3.jpg') },
        { hid: 'description', name: 'description', content: '三民家商「綠意的環抱」' },
        { hid: 'og:description' , property: 'og:description' , content: '三民家商「綠意的環抱」' },
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
      detail: { img: require('@/assets/img/article/s02/3.jpg'), position: 'r', type: 'h', name: '三民家商', place: 's', title: '綠意的環抱', desc: '馨語', content: '生活之快速，是否能夠停下腳步？在這閱讀，涼爽的微風會穿過你的身旁，綠意將會包圍著你，在此沈浸在閱讀的美好吧！', link: '30203' }
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