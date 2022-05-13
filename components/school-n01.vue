<template>
  <div>
    <schoolContain :title="title" :frames="frames" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '輔大聖心高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '輔大聖心高中' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n01/1.jpg') },
        { hid: 'description', name: 'description', content: '天主教基隆市輔大聖心高級中學' },
        { hid: 'og:description' , property: 'og:description' , content: '天主教基隆市輔大聖心高級中學' },
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
      title: '輔大聖心高中',
      frames: [
        { img: require('@/assets/img/article/n01/1.jpg'), title: '操場也能閱讀？閱讀無限', desc: 'HYC' },
        { img: require('@/assets/img/article/n01/2.jpg'), title: '閱在花中', desc: '三口' }
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