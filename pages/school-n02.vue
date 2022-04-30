<template>
  <div>
    <schoolContain :title="title" :frames="frames" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '臺灣大學',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '臺灣大學' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n-01_s01_01.jpeg') },
        { hid: 'description', name: 'description', content: '國立臺灣大學' },
        { hid: 'og:description' , property: 'og:description' , content: '國立臺灣大學' },
      ],
    }
  },
  layout: 'default',
  components: {
    schoolContain: require('~/components/school-contain.vue').default,
  },
  props: {
    
  },
  data () {
    return {
      title: '臺灣大學',
      frames: [
        { img: require('@/assets/img/article/n-02_u01_01.jpg'), title: '靜閱', desc: '洗硯' }
      ]
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