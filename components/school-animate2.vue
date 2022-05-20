<template>
  <div class="animate2">
    <div class="animate2-bg"></div>
    <div class="animate2-school"></div>
    <div class="animate2-door"></div>
    <div class="animate2-tree"></div>
    <div class="animate2-name">{{ title }}</div>
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

.animate2 {
  position: fixed;
  left: 0px;
  top: 0px;
  width: 100vw;
  height: 100vh;
  background-color: white;
  z-index: 2;

  &-bg {
    position: absolute;
    left: 0px;
    top: 0px;
    width: 100vw;
    height: 100vh;
    background-image: url('../assets/img/animate/university/bg.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-school {
    position: absolute;
    left: 0px;
    bottom: 0px;
    width: 100%;
    height: 100%;
    background-image: url('../assets/img/animate/university/university.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-door {
    position: absolute;
    left: calc(47%);
    top: calc(60%);
    width: 10%;
    height: 20%;
    background-image: url('../assets/img/animate/university/run.gif');
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-tree {
    position: absolute;
    left: 0px;
    bottom: 0;
    width: 100vw;
    height: 38vh;
    background-image: url('../assets/img/animate/university/tree.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-name {
    position: absolute;
    left: calc(51% - 120px);
    top: 42%;
    width: 240px;
    height: 60px;
    line-height: 60px;
    text-align: center;
    font-size: 32px;
    font-weight: bold;
    border: 1px solid black;
    background-color: white;
  }
}



@media( max-width: 1023px ){

.animate2 {

  &-bg {
    left: 0px;
    top: 0px;
    width: 100vw;
    height: 100vh;
    background-image: url('../assets/img/animate/university/bg-m.png');
  }

  &-school {
    // left: calc(0px);
    // top: calc(0%);
    // width: 100%;
    // height: 100%;
    // background-image: url('../assets/img/animate/university/university-m.png');
  }

  &-door {
    left: calc(50% - 40px);
    top: 62%;
    width: 115px;
    height: 135px;
    background-image: url('../assets/img/animate/university/run.gif');
  }

  &-tree {
    left: 0px;
    bottom: 0%;
    width: 100vw;
    height: 22vh;
    background-image: url('../assets/img/animate/high/tree-m.png');
  }

  &-name {
    left: calc(50% - 90px);
    top: 40%;
    width: 180px;
    height: 46px;
    line-height: 46px;
    font-size: 24px;
  }
}

}

@media( max-width: 332px ){

.animate2 {

  &-school {

  }

  &-door {

  }
}

}

</style>