<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '三民家商',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/s02/1.jpg') },
        { hid: 'description', name: 'description', content: '三民家商「馨園」' },
        { hid: 'og:description' , property: 'og:description' , content: '三民家商「馨園」' },
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
      detail: { img: require('@/assets/img/article/s02/1.jpg'), position: 'r', type: 'h', name: '三民家商', place: 's', title: '馨園', desc: '馨語', content: '學校的秘密花園，宛如置身夢境中的森林，投入大自然的環抱，悠閒的午後最適合停留在此閱讀，空氣中的芬多精與此起彼落的鳥鳴聲將會是陪伴你陶醉文字的最佳夥伴。', link: '30201' }
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