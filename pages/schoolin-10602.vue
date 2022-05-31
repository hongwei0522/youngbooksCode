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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n06/2.jpg') },
        { hid: 'description', name: 'description', content: '再興中學「有一個角落」' },
        { hid: 'og:description' , property: 'og:description' , content: '再興中學「有一個角落」' },
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
      detail: { img: require('@/assets/img/article/n06/2.jpg'), position: 'v', name: '再興中學', place: 'n', title: '有一個角落', desc: 'Jordan.W', content: '有一個角落，能夠讓我放鬆下心情，享受著微風輕輕拂過我的臉龐，讓風把一切的思緒都帶走，只留下無憂無慮的我和這短暫的自由。', link: '10602' }
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