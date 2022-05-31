<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '北港高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/m05/1.jpg') },
        { hid: 'description', name: 'description', content: '北港高中「野生閱讀私角落」' },
        { hid: 'og:description' , property: 'og:description' , content: '北港高中「野生閱讀私角落」' },
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
      detail: { img: require('@/assets/img/article/m05/1.jpg'), position: 'r', type: 'h', name: '北港高中', place: 'm', title: '野生閱讀私角落', desc: '詩乃萬歲', content: '坐鎮於學校東南隅的天佑沙崗石的背後，視野遼闊，人煙罕至，綠意盎然，花鳥扶疏，置身這充滿著野生氣息的桃花源中，不管是在這用功讀書或思考人生，都能怡然自得，事半功倍。每當處於此時，背後那蘶峨巨石的氣勢與遍地小草的柔情相衝之下總會讓我舒筋展骨，酣暢淋漓。對未來感到迷惘時來這裡，雖無法悟出如天地沙鷗的感慨，但是仍然可以讓心情舒服許多。', link: '20501' }
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