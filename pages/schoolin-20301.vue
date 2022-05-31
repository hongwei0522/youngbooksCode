<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '西苑高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/m03/1.jpg') },
        { hid: 'description', name: 'description', content: '西苑高中「心中角落」' },
        { hid: 'og:description' , property: 'og:description' , content: '西苑高中「心中角落」' },
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
      detail: { img: require('@/assets/img/article/m03/1.jpg'), position: 'v', type: 'h', name: '西苑高中', place: 'm', title: '心中角落', desc: '姍姍', content: '這是校園中人最少的樓梯間，我喜歡這裡的安靜，後牆上貼著的勵志標語，閱讀是自己的私有空間，有自己的秘密，因此我喜歡安靜在這閱讀，施肥於心中淨土，偶爾在中午時會有陽光灑下，很溫暖，坐在樓梯間看著剛從圖書館借來的書籍，是那一天最享受的事，以這張沒有甚麼修過的照片，分享給大家最自然的閱讀空間。', link: '20301' }
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