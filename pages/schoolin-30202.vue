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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s02/2.jpg') },
        { hid: 'description', name: 'description', content: '三民家商「春日閱讀」' },
        { hid: 'og:description' , property: 'og:description' , content: '三民家商「春日閱讀」' },
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
      detail: { img: require('@/assets/img/article/s02/2.jpg'), position: 'r', type: 'h', name: '三民家商', place: 's', title: '春日閱讀', desc: '馨語', content: '結束忙碌的一天不妨與生活借些時間閱讀，在室內設計辦公室的後花園裡能夠感受到無比的遼闊，讀累了就選擇抬頭望天空，天藍色的美景與瞬息萬變的雲朵盡收眼底。', link: '30202' }
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