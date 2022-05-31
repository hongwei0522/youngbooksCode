<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '新營高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s01/6.jpg') },
        { hid: 'description', name: 'description', content: '新營高中「閱讀秘境」' },
        { hid: 'og:description' , property: 'og:description' , content: '新營高中「閱讀秘境」' },
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
      detail: { img: require('@/assets/img/article/s01/6.jpg'), position: 'r', type: 'h', name: '新營高中', place: 's', title: '閱讀秘境', desc: 'Ruby', content: '學校隱密的通道通向安靜清幽的涼亭，午後最適合在那裏享受閱讀的樂趣，微風徐徐，良好的閱讀環境紓解課業，使我每天上學都能元氣十足。木製的涼亭融合後方的樹木，就像和大自然一起閱讀，陽光穿透樹葉灑在長椅上，那樣的繽紛絢麗是無可取代的。', link: '30106' }
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