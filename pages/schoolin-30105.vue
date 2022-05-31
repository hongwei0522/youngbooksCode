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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s01/5.jpg') },
        { hid: 'description', name: 'description', content: '新營高中「閱讀小工坊」' },
        { hid: 'og:description' , property: 'og:description' , content: '新營高中「閱讀小工坊」' },
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
      detail: { img: require('@/assets/img/article/s01/5.jpg'), position: 'v', type: 'h', name: '新營高中', place: 's', title: '閱讀小工坊', desc: '小菜', content: '學校的圖書館旁有一間小木屋，裡面有著木頭的香味，眼前的落地窗能將面前美好的風景盡收眼底，讓人自由自在的在書海暢遊，屏蔽外界的紛擾！', link: '30105' }
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