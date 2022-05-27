<template>
  <div class="top-title">
    <div>{{ this.title }}</div>
    <!-- <div>閱讀私角落</div>
    <div>校園攝影展</div> -->
  </div>
</template>

<script>
export default {
  components: {

  },
  props: {
    title: {
      type: String
    }
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

<style lang="scss">

.top-title {
    display: flex;
    justify-content: center;
    margin: 20px 0px 0px;
    font-size: 48px;

    // & div:first-child {
    //   margin-right: 60px;
    // }

    // & div:nth-child(2) {
    //   margin-right: 60px;
    // }
  }

@media( max-width: 1023px ){

  .top-title {
    flex-wrap: wrap;
    align-items: center;
    margin: 60px 0px 0px;
    font-size: 30px;

    // & div:first-child {
    //   width: 100%;
    //   text-align: center;
    //   margin-right: 0px;
    // }

    // & div:nth-child(2) {
    //   margin-right: 10px;
    // }
  }

}


</style>