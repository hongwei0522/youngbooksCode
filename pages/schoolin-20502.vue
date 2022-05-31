<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '北港高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/m05/2.jpg') },
        { hid: 'description', name: 'description', content: '北港高中「窗邊閱讀私角落」' },
        { hid: 'og:description' , property: 'og:description' , content: '北港高中「窗邊閱讀私角落」' },
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
      detail: { img: require('@/assets/img/article/m05/2.jpg'), position: 'v', type: 'h', name: '北港高中', place: 'm', title: '窗邊閱讀私角落', desc: '北高彭于晏', content: '美好的靠窗座位，是段考前十名所帶給我的選位權利，將來大概會繼續留在此處直到畢業使我和它分離。除了可欣賞窗外路過的美女們，窗戶一開，即有悅耳的啁啾聲傳入耳中，宜人的微風吹動髮絲；深綠的窗簾一拉開，陽光可直接明亮我的世界，日光燈即失去它的作用。不用咖啡和輕音樂，背靠窗台翹起腳，便留給外頭走廊一個文青的背影。', link: '20502' }
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