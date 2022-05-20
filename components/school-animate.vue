<template>
  <div class="animate">
    <div class="animate-bg"></div>
    <div class="animate-school"></div>
    <div class="animate-door"></div>
    <div class="animate-tree"></div>
    <div class="animate-name">{{ title }}</div>
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

.animate {
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
    background-image: url('../assets/img/animate/high/bg.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-school {
    position: absolute;
    left: calc(50% - 400px);
    top: calc(50% - 350px);
    width: 800px;
    height: 700px;
    background-image: url('../assets/img/animate/high/high-school.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-door {
    position: absolute;
    left: calc(50% - 70px);
    top: calc(54%);
    width: 150px;
    height: 150px;
    background-image: url('../assets/img/animate/high/run.gif');
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-tree {
    position: absolute;
    left: 0px;
    bottom: 10%;
    width: 100vw;
    height: 38vh;
    background-image: url('../assets/img/animate/high/tree.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-name {
    position: absolute;
    left: calc(50% - 120px);
    top: 41%;
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

.animate {

  &-bg {
    left: 0px;
    top: 0px;
    width: 100vw;
    height: 100vh;
    background-image: url('../assets/img/animate/high/bg-m.png');
  }

  &-school {
    left: calc(50% - 200px);
    top: calc(50% - 150px);
    width: 400px;
    height: 300px;
    background-image: url('../assets/img/animate/high/high-school-m.png');
  }

  &-door {
    left: calc(50% - 48px);
    top: calc(48%);
    width: 110px;
    height: 120px;
    background-image: url('../assets/img/animate/high/run.gif');
  }

  &-tree {
    left: 0px;
    bottom: 24%;
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

</style>