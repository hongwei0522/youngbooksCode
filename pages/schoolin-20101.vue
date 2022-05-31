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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/m01/1.jpg') },
        { hid: 'description', name: 'description', content: '三義高中「閱幸福越青春」' },
        { hid: 'og:description' , property: 'og:description' , content: '三義高中「閱幸福越青春」' },
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
      detail: { img: require('@/assets/img/article/m01/1.jpg'), position: 'v', type: 'h', name: '三義高中', place: 'm', title: '閱幸福越青春', desc: '王玉萱', content: '在涵美樓3樓較少人走動的長廊，吹著徐徐的微風，眼前環繞著群山和雲朵。天氣晴朗時還能遠望「雪山」的尊貴。陽光灑落在書面上，配上這片風景，讓我能盡情的閱讀，疲倦時還能抬頭欣賞美景和讓眼睛休息。', link: '20101' }
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