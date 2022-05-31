<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '桃園陽明高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n09/2.jpg') },
        { hid: 'description', name: 'description', content: '桃園陽明高中「我的世外桃源」' },
        { hid: 'og:description' , property: 'og:description' , content: '桃園陽明高中「我的世外桃源」' },
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
      detail: { img: require('@/assets/img/article/n09/2.jpg'), position: 'r', name: '桃園陽明高中', place: 'n', title: '我的世外桃源', desc: '四加減雲', content: '操場同學們開朗的笑聲，微風徐來吹拂，樹葉窸窣作響，伴坐在榕樹下享受美好閱讀時光。我如桃源武陵人，忘卻一切的煩憂，在此豁然開朗，更享受自然的交響樂，因為這裡專屬於我的世外桃源。', link: '10902' }
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