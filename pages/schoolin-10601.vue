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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n06/1.jpeg') },
        { hid: 'description', name: 'description', content: '再興中學「秋」' },
        { hid: 'og:description' , property: 'og:description' , content: '再興中學「秋」' },
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
      detail: { img: require('@/assets/img/article/n06/1.jpeg'), position: 'r', name: '再興中學', place: 'n', title: '秋', desc: '珈安', content: '在秋天的黃昏，坐在凳子上，看著太陽漸漸落下帷幕，是多麼美好的時刻，恍然體會到書上描寫的美景竟是真實存在，我想我應該穿越書裡的世界了吧！', link: '10601' }
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