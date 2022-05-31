<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '士林高商',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n08/6.jpg') },
        { hid: 'description', name: 'description', content: '士林高商「祈福的願望」' },
        { hid: 'og:description' , property: 'og:description' , content: '士林高商「祈福的願望」' },
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
      detail: { img: require('@/assets/img/article/n08/6.jpg'), position: 'r', name: '士林高商', place: 'n', title: '祈福的願望', desc: 'Yh_', content: '這一塊塊木製板，不僅是目標、願望，還是承載著夢想的初心。', link: '10806' }
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