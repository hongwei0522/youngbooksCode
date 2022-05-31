<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '再興中學',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n06/4.jpg') },
        { hid: 'description', name: 'description', content: '再興中學「下課十分鐘」' },
        { hid: 'og:description' , property: 'og:description' , content: '再興中學「下課十分鐘」' },
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
      detail: { img: require('@/assets/img/article/n06/4.jpg'), position: 'v', name: '再興中學', place: 'n', title: '下課十分鐘', desc: 'Jordan.W', content: '下課十分鐘，在教室享受著陽光，翻開上次未閱讀完的章節，沉浸在屬於我一個人的休息時光。', link: '10604' }
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