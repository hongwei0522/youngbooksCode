<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '臺灣大學',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n02/1.jpg') },
        { hid: 'description', name: 'description', content: '臺灣大學「靜閱」' },
        { hid: 'og:description' , property: 'og:description' , content: '臺灣大學「靜閱」' },
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
      detail: { img: require('@/assets/img/article/n02/1.jpg'), positon: 'v', name: '臺灣大學', place: 'n', title: '靜閱', desc: '洗硯', content: '時光在普通大樓2樓的戶外空間以徐緩的速度流淌，靜靜坐在木椅上，和著花草點綴徜徉在文字之中，暫時拋開了外頭喧囂，在這樣的角落中擁有一個靜慢而綠意盎然的宇宙，如花草般春意盎然，生生不息。', link: '10201' }
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