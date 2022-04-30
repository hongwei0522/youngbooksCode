<template>
  <div class="index">
    <div class="index-outer">

      <topBar/>

      <div class="index-intro">
        <div class="index-intro-title">閱讀私角落　校園攝影展</div>
        <div>
          <div class="index-intro-text">
            <div>有一個角落，可以自由呼吸</div>
            <div>有一個角落，可以滋養閱讀</div>
          </div>
          <div class="index-intro-text">
            <div>有一個角落，可以支持我</div>
            <div>讓陽光灑落，可以孤單不會孤獨</div>
          </div>
          <div class="index-intro-text">可以一個人，可以一群人</div>
          <div class="index-intro-text">我最喜歡的校園空間、支持你的閱讀私角落</div>
        </div>
      </div>

      <div class="index-map-tag">
        <div class="index-map">

        </div>
        <div class="index-tag">
          <selectSption />
          <div class="index-tag-box">
            <nuxt-link class="index-tag-link" to="/school">
              <div class="index-tag-text">#長樂國小</div>
            </nuxt-link>
            <nuxt-link class="index-tag-link" to="/school-n01">
              <div class="index-tag-text">#輔大聖心高中</div>
            </nuxt-link>
            <nuxt-link class="index-tag-link" to="/school-n02">
              <div class="index-tag-text">#臺灣大學</div>
            </nuxt-link>
          </div>
        </div>
      </div>


    </div>
    
  </div>
</template>

<script>
export default {
  layout: 'default',
  components: {
    topBar: require('~/components/top-bar.vue').default,
    selectSption: require('~/components/select-option.vue').default,
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

.index {
  background-image: url('../assets/img/index/bg-pc.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position-x: center;
  background-position-y: center;
  width: calc(100% - 40px);
  min-height: 100vh;
  display: flex;
  justify-content: center;

  &-outer {
    max-width: 1400px;
    width: 100%;
    padding: 0px 20px;
  }

  &-header {
    

  }

  &-intro {
    display: flex;
    flex-direction: column;
    align-items: center;

    &-title {
      margin: 40px 0px 45px;
      font-size: 48px;
    }

    &-text {
      font-weight: 100;

      &:nth-child(1) {
        display: flex;
        font-weight: 300;

        & div:first-child {
          margin-right: 50px;
        }
      }

      &:nth-child(2) {
        display: flex;

        & div:first-child {
          margin-right: 50px;
        }
      }
    }
  }

  &-map-tag {
    display: flex;
    justify-content: center;
  }

  &-map {
    width: 50%;
    height: 600px;
    margin-top: 50px;
    background-color: red;
  }

  &-tag {
    width: 50%;
    margin-top: 160px;

    &-box {
      margin-top: 30px;
    }

    &-link {

    }

    &-text {
      font-size: 30px;
      font-weight: bold;
      color: #779862;
    }
  }

}


</style>

