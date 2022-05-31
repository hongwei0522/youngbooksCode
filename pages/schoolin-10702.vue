<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '中山女高',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n07/2.jpg') },
        { hid: 'description', name: 'description', content: '中山女高「青春與閱讀的相遇」' },
        { hid: 'og:description' , property: 'og:description' , content: '中山女高「青春與閱讀的相遇」' },
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
      detail: { img: require('@/assets/img/article/n07/2.jpg'), position: 'v', name: '中山女高', place: 'n', title: '青春與閱讀的相遇', desc: '小韌', content: '在學校中央的大草皮上，<br>我們揮擲青春年華，<br>或追逐嬉戲，或圍圈談心，或翻開扉頁盡情閱讀，<br>都交織出女校生活裡最難忘與快樂的回憶點滴。', link: '10702' }
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