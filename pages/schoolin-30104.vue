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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s01/4.jpg') },
        { hid: 'description', name: 'description', content: '新營高中「閱讀森林」' },
        { hid: 'og:description' , property: 'og:description' , content: '新營高中「閱讀森林」' },
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
      detail: { img: require('@/assets/img/article/s01/4.jpg'), position: 'v', type: 'h', name: '新營高中', place: 's', title: '閱讀森林', desc: '小菜', content: '學校的鞦韆旁有許許多多的大樹，讓人彷彿置身於森林中，坐在鞦韆上讀書讀累了就欣賞一下附近那些綠意盎然的樹，這種讀書的氛圍讓人感到很放鬆，但，同時又能進入自己的小小世界！', link: '30104' }
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