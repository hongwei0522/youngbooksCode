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
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n09/1.jpg') },
        { hid: 'description', name: 'description', content: '桃園陽明高中「專屬的閱讀角落」' },
        { hid: 'og:description' , property: 'og:description' , content: '桃園陽明高中「專屬的閱讀角落」' },
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
      detail: { img: require('@/assets/img/article/n09/1.jpg'), position: 'r', name: '桃園陽明高中', place: 'n', title: '專屬的閱讀角落', desc: '艾琳', content: '恰到好處的桌椅、清新的空氣、一本本系列小說，徜徉在書海就是最享受的事情。沉浸在這裡看書，能夠讓瞬間人忘了考試報告的壓力、人際交往的煩惱甚至是時間的流逝。這個角落就是陽明高中的最高層樓，是放鬆心情、抒發壓力的好去處，是煩悶解壓的好場所，也是我專屬的閱讀小角落。', link: '10901' }
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