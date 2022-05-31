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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n07/1.jpg') },
        { hid: 'description', name: 'description', content: '中山女高「背光」' },
        { hid: 'og:description' , property: 'og:description' , content: '中山女高「背光」' },
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
      detail: { img: require('@/assets/img/article/n07/1.jpg'), position: 'v', name: '中山女高', place: 'n', title: '背光', desc: '羅宜蓁', content: '教室中的白光變得有些煩膩，是時候逃離水泥的僵硬奔向千變萬化的自然和煦，<br>踏上灑上數點綠油的中山草皮，一片片稀疏錯落的繁花簇擁，綠意盎然，<br>舉起書本向臉上一放，仰頭，<br>背著光，卻看見更加清晰的文字烙印；<br>背著光，卻意外住進一頂天空的蔚藍。', link: '10701' }
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