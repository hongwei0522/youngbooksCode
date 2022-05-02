<template>
  <div class="header">
    
    <a class="header-link" href="https://ireader.books.com.tw/" target="_blank">
      <img class="header-logo" src="@/assets/img/icon/logo.png" alt="logo">
    </a>
    <a class="header-link" href="https://www.facebook.com/books.youth" target="_blank">
      <img class="header-social" src="@/assets/img/icon/fb.png" alt="fb">
    </a>
    <a class="header-link" href="https://www.instagram.com/books.youth/" target="_blank">
      <img class="header-social" src="@/assets/img/icon/ig.png" alt="ig">
    </a>
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

.header {
  margin-top: 28px;

  &-link {
    
  }

  &-logo {
    width: 224px;
    height: 100%;
    margin-right: 20px;
  }

  &-social {
    width: 30px;
    height: 100%;
    margin: 0px 7px 4px 0px;
  }
}

@media( max-width: 1023px ){

.header {
  margin-top: 10px;

  &-link {
    
  }

  &-logo {
    width: 200px;
    margin-right: 6px;
  }

  &-social {
    width: 26px;
    margin: 0px 7px 6px 0px;
  }
}

}


</style>