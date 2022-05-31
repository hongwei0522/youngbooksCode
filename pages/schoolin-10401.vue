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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n04/1.jpg') },
        { hid: 'description', name: 'description', content: '臺北市大「燈下書香」' },
        { hid: 'og:description' , property: 'og:description' , content: '臺北市大「燈下書香」' },
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
      detail: { img: require('@/assets/img/article/n04/1.jpg'), position: 'r', name: '臺北市大', place: 'n', title: '燈下書香', desc: '麻糬', content: '窩在圖書館的一角，點亮桌上的一盞燈，翻開一本書，安閒自在地度過一個早晨，享受獨處的時光。', link: '10401' }
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