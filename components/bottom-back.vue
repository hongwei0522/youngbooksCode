<template>
  <div class="bottom-back">
    <nuxt-link to="/">
      <div class="bottom-back-btn">
        <div>看其他學校</div>
        <img class="bottom-back-icon" src="@/assets/img/icon/go-arrow.png" alt="arrow back">
      </div>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  components: {

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

<style lang="scss">

.bottom-back {
  display: flex;
  justify-content: flex-end;
  margin: 30px 0px 10px 0px;

  &-btn {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 346px;
    padding: 4px 0px;
    text-align: center;
    font-size: 36px;
    color: black;
    background: #D8D76F;
    border-radius: 50px;
    cursor: pointer;

    &:hover {
      opacity: 0.8;
    }
  }

  &-icon {
    width: 14px;
    height: 100%;
    margin: 4px 0px 0px 10px;
  }
}

@media( max-width: 1023px ){

  .bottom-back {
    justify-content: center;

    &-btn {
      width: 260px;
      font-size: 24px;
    }

    &-icon {
      width: 10px;
    }
  }

}

</style>