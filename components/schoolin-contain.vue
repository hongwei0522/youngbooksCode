<template>
  <div class="schoolin">
    <div class="schoolin-outer">
      <topBar/>
      <titleBar :title="this.name" />

      <div class="schoolin-inner">

        <div class="schoolin-left">
          <div :style="[ isSquare ? 
            {'backgroundImage' : 'url(' + require('@/assets/img/schoolin/photo-row.png') + ')'} : '' 
          ]"
            :class="['schoolin-frame',
              {'schoolin-frame-square': isSquare}
            ]"
          >
            <div :style="{
              'backgroundImage' : 'url(' + detail.img + ')'
            }"
              :class="['schoolin-photo',
                {'schoolin-photo-square': isSquare}
              ]"
            ></div>
          </div>
        </div>

        <div class="schoolin-right">
          <div class="schoolin-head">{{ detail.title }}</div>
          <div class="schoolin-sub">{{ detail.desc }}</div>
          <div class="schoolin-line"></div>
          <div class="schoolin-text" v-html="detail.content"></div>
          <div class="schoolin-line"></div>

          <div class="schoolin-social">
            <img @click="copy()" class="schoolin-icon" src="@/assets/img/icon/copy.png" alt="copy link">
            <a :href="`https://social-plugins.line.me/lineit/share?url=${currentUrl}`" target="_blank">
              <img class="schoolin-icon" src="@/assets/img/icon/line-share.png" alt="share line">
            </a>
            <a :href="`https://www.facebook.com/sharer/sharer.php?u=${fbUrl}&amp;src=sdkpreparse`" target="_blank">
              <img class="schoolin-icon" src="@/assets/img/icon/fb-share.png" alt="share fb">
            </a>
          </div>

          <bottomBack />

        </div>
      </div>

      
    </div>
  </div>
</template>

<script>
export default {
  components: {
    topBar: require('~/components/top-bar.vue').default,
    titleBar: require('~/components/title-bar.vue').default,
    bottomBack: require('~/components/bottom-back.vue').default,
  },
  props: {
    detail: {
      type: Object
    },
  },
  data () {
    return {
      name: '長樂國小',
      currentUrl: '',
      fbUrl: '',
      isSquare: false,
      frame: '',
    }
  },
  mounted () {
    this.currentUrl = window.location.href
    this.fbUrl = window.location.href
    this.fbUrl = this.fbUrl.replaceAll('/', '%2F')

    this.name = this.detail.name
    if(this.detail.position == 'r') {
      this.isSquare = true
    }
  },
  computed: {

  },
  methods: {
    copy(){
      var domUrl = document.createElement("input");
      domUrl.value = this.currentUrl;
      domUrl.id = "creatDom";
      document.body.appendChild(domUrl);
      domUrl.select(); // 选择对象
      document.execCommand("Copy"); // 执行浏览器复制命令
      let creatDom = document.getElementById("creatDom");
      creatDom.parentNode.removeChild(creatDom);
      this.$message({
          message: '複製成功',
          type: 'success'
      });
    }
  },
  watch: {
    
  }
}
</script>

<style lang="scss" scoped>

.schoolin {
  background-image: url('../assets/img/school/bg-pc.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position-x: center;
  background-position-y: center;
  min-height: 100vh;
  display: flex;
  justify-content: center;

  &-outer {
    max-width: 1400px;
    width: calc(100% - 100px);
    padding: 0px 50px;
  }

  &-inner {
    display: flex;

  }

  &-left {
    
  }

  &-frame {
    width: 400px;
    height: 530px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: url('../assets/img/schoolin/photo-straight.png');
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-frame-square {
    height: 330px;
  }

  &-photo {
    width: 360px;
    height: 490px;
    background-repeat: no-repeat;
    background-size: cover;
    background-position-x: center;
    background-position-y: center;
  }

  &-photo-square {
    width: 350px;
    height: 264px;
  }

  &-right {
    width: 100%;
    margin-left: 30px;
  }

  &-head {
    font-size: 30px;
  }

  &-sub {
    font-size: 18px;
  }

  &-line {
    margin: 12px 0px;
    border-bottom: 1px solid black;
  }

  &-text {
    font-size: 24px;
  }

  &-social {
    
  }

  &-icon {
    width: 40px;
    height: 40px;
    margin-right: 4px;
    cursor: pointer;
  }
}

@media( max-width: 1023px ){

  .schoolin {
    background-image: url('../assets/img/school/bg-m.jpg');

    &-outer {
      width: calc(100% - 10px);
      padding: 0px 5px;
    }

    &-inner {
      flex-direction: column;
      margin-top: 25px;
    }

    &-left {
      margin: auto;
    }

    &-frame {
      width: 310px;
      height: 410px;
    }

    &-frame-square {
      width: 315px;
      height: 225px;
    }

    &-photo {
      width: 260px;
      height: 360px;
    }

    &-photo-square {
      width: 248px;
      height: 182px;
    }

    &-right {
      width: calc(100% - 80px);
      margin: 0px;
      padding: 0px 40px;
    }

    &-head {
      font-size: 20px;
      margin-top: 30px;
    }

    &-sub {
      font-size: 16px;
    }

    &-line {
      
    }

    &-text {
      font-size: 18px;
    }

    &-social {
      text-align: right;
    }

    &-icon {
      
    }

  }
}

</style>