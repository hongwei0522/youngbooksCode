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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s02/4.jpg') },
        { hid: 'description', name: 'description', content: '三民家商「閱讀長凳」' },
        { hid: 'og:description' , property: 'og:description' , content: '三民家商「閱讀長凳」' },
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
      detail: { img: require('@/assets/img/article/s02/4.jpg'), position: 'r', type: 'h', name: '三民家商', place: 's', title: '閱讀長凳', desc: '馨語', content: '不需要良辰吉時，在此，任何時刻都能讓人感到沁涼舒服，有時暖暖的陽光從籬笆縫透了出來，彷彿在支持你繼續留在原地閱讀，在悠閒的時刻坐在長凳上閱讀將會是最佳的選擇。', link: '30204' }
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