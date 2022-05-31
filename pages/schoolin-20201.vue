<template>
  <div>
    <schoolinContain :detail="detail" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: '新社高中',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '青春博客來閱讀私角落' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/m02/1.jpg') },
        { hid: 'description', name: 'description', content: '新社高中「寧靜的午後時光」' },
        { hid: 'og:description' , property: 'og:description' , content: '新社高中「寧靜的午後時光」' },
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
      detail: { img: require('@/assets/img/article/m02/1.jpg'), position: 'v', type: 'h', name: '新社高中', place: 'm', title: '寧靜的午後時光', desc: 'Sam', content: '在中午過後的學校裡，充滿著溫暖的陽光與寧靜的時光，在此時拿起一本自己喜歡的書閱讀吧！', link: '20201' }
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