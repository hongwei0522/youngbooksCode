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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s01/1.jpeg') },
        { hid: 'description', name: 'description', content: '新營高中「沉浸」' },
        { hid: 'og:description' , property: 'og:description' , content: '新營高中「沉浸」' },
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
      detail: { img: require('@/assets/img/article/s01/1.jpeg'), position: 'v', type: 'h', name: '新營高中', place: 's', title: '沉浸', desc: 'Giga', content: '整天不僅沉浸在書本裡，也沉浸在這美麗的校園', link: '30101' }
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