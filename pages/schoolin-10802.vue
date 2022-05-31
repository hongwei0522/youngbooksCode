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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n08/2.jpg') },
        { hid: 'description', name: 'description', content: '士林高商「滄海一栗」' },
        { hid: 'og:description' , property: 'og:description' , content: '士林高商「滄海一栗」' },
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
      detail: { img: require('@/assets/img/article/n08/2.jpg'), position: 'r', name: '士林高商', place: 'n', title: '滄海一栗', desc: '狐狸', content: '從地面的角度看上去，人就像小小的一粒米在廣大的書海中飄遊著，被包裹在常常得書的走廊另一個盡頭', link: '10802' }
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