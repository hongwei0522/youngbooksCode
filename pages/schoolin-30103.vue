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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s01/3.jpg') },
        { hid: 'description', name: 'description', content: '新營高中「我的閱讀角落」' },
        { hid: 'og:description' , property: 'og:description' , content: '新營高中「我的閱讀角落」' },
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
      detail: { img: require('@/assets/img/article/s01/3.jpg'), position: 'v', type: 'h', name: '新營高中', place: 's', title: '我的閱讀角落', desc: '陳宜庭', content: '學校的每個小角落,都是我增長知識的小天地', link: '30103' }
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