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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s01/2.jpg') },
        { hid: 'description', name: 'description', content: '新營高中「被藏匿的烏托邦」' },
        { hid: 'og:description' , property: 'og:description' , content: '新營高中「被藏匿的烏托邦」' },
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
      detail: { img: require('@/assets/img/article/s01/2.jpg'), position: 'v', type: 'h', name: '新營高中', place: 's', title: '被藏匿的烏托邦', desc: '小一', content: '在平日的下午，我身在圖書館前的一座小石椅上，心賞眼前的一片風景，閱覽著富含豐富知識的英文雜誌，愜意地感受風吹拂著臉龐，此刻的我，感到非常的幸福。', link: '30102' }
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