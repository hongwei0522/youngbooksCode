<template>
  <div>
    <schoolContain :title="title" :frames="frames" />
  </div>
</template>

<script>
export default {
  head() {
    return {
      
    }
  },
  layout: 'default',
  components: {
    schoolContain: require('~/components/school-contain.vue').default,
  },
  props: {
    
  },
  data () {
    return {
      
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