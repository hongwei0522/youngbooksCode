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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n08/7.jpg') },
        { hid: 'description', name: 'description', content: '士林高商「吾師」' },
        { hid: 'og:description' , property: 'og:description' , content: '士林高商「吾師」' },
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
      detail: { img: require('@/assets/img/article/n08/7.jpg'), position: 'v', name: '士林高商', place: 'n', title: '吾師', desc: '花生俠', content: '在讀書館研讀時，常常會看到打哈欠，但一想到孔子在一旁注視著我，讀書的熱忱好像又湧上來了。', link: '10807' }
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