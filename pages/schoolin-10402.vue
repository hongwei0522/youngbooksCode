<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '臺北市大',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n04/2.jpg') },
        { hid: 'description', name: 'description', content: '臺北市大「窗前書香」' },
        { hid: 'og:description' , property: 'og:description' , content: '臺北市大「窗前書香」' },
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
      detail: { img: require('@/assets/img/article/n04/2.jpg'), position: 'r', name: '臺北市大', place: 'n', title: '窗前書香', desc: '麻糬', content: '站在走廊盡頭的窗邊，能看見校園景色、聞鳥語花香、感受微風輕拂臉頰、沉澱心靈、恢復疲憊的身心靈、滿血復活。', link: '10402' }
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