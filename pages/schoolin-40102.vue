<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '慈大附中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/e01/2.jpeg') },
        { hid: 'description', name: 'description', content: '慈大附中「第二閱讀儀式感」' },
        { hid: 'og:description' , property: 'og:description' , content: '慈大附中「第二閱讀儀式感」' },
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
      detail: { img: require('@/assets/img/article/e01/2.jpeg'), position: 'v', type: 'h', name: '慈大附中', place: 'e', title: '第二閱讀儀式感', desc: '兀', content: '一聲清晨五點鐘的鬧鐘，一個慵懶的哈欠，一杯溫開水，幾本準備複習預習的書，是我開啟一整天美好的閱讀儀式感。早起養成的習慣，使我幸運能享受特別待遇，接受到教室第一道光的迎接，沐浴在陽光的洗禮，每日早晨七點鐘的那道光，是我的第二個閱讀儀式感。', link: '40102' }
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