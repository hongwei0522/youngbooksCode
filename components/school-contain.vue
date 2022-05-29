<template>
  <div class="school">
    <div class="school-outer">
      <topBar/>
      <titleBar :title="this.title" />

      <!-- 手機版 & 三個(以上)的版本，有 loop -->  
      <div v-if="frames.length >= 3 || currentWidth < 1024" class="school-swiper-outer-box">
        <swiper class="swiper school-swiper" :options="swiperOption" ref="mySwiper">
          <swiper-slide class="school-swiper-slide"
            v-for="(frame, index) in frames"
            :key="index"
          >
            <nuxt-link :to="`/schoolin-${frame.link}`">
              <div class="school-swiper-bg">
                <div class="school-swiper-box">
                  <div class="school-swiper-img"
                    :style="[
                      {'backgroundImage': 'url(' + frame.img + ')'}
                    ]"
                  ></div>
                  <div class="school-swiper-title">{{ frame.title }}</div>
                  <div class="school-swiper-desc">{{ frame.desc }}</div>
                </div>
              </div>
            </nuxt-link>
          </swiper-slide>
        </swiper>
          <img v-if="slide.isShowPrev" @click="prevSlide()" class="school-swiper-prev" src="@/assets/img/icon/left-arrow.png" alt="prev">
          <img v-if="slide.isShowNext" @click="nextSlide()" class="school-swiper-next" src="@/assets/img/icon/right-arrow.png" alt="next">
      </div>

      <!-- 桌面版一個、兩個，沒有 loop -->
      <div v-else class="school-swiper-outer-box">
        <swiper class="swiper school-swiper" :options="swiperOption2" ref="mySwiper">
          <swiper-slide class="school-swiper-slide"
            v-for="(frame, index) in frames"
            :key="index"
          >
            <nuxt-link :to="`/schoolin-${frame.link}`">
              <div class="school-swiper-bg">
                <div class="school-swiper-box">
                  <div class="school-swiper-img"
                    :style="[
                      {'backgroundImage': 'url(' + frame.img + ')'}
                    ]"
                  ></div>
                  <div class="school-swiper-title">{{ frame.title }}</div>
                  <div class="school-swiper-desc">{{ frame.desc }}</div>
                </div>
              </div>
            </nuxt-link>
          </swiper-slide>
        </swiper>
      </div>

      <bottomBack />

    </div>
  </div>
</template>

<script>
export default {
  components: {
    topBar: require('~/components/top-bar.vue').default,
    titleBar: require('~/components/title-bar.vue').default,
    bottomBack: require('~/components/bottom-back.vue').default,
    selectSption: require('~/components/select-option.vue').default,
  },
  props: {
    frames: {
      type: Array
    },
    title: {
      type: String
    }
  },
  data () {
    return {
      slide: {
        total: 0,
        current: 0,
        isShowPrev: true,
        isShowNext: true
      },
      currentWidth: null,
      //  手機版 & 三個(以上)的版本，有 loop
      swiperOption: {
        // scrollbar: true,
        // mousewheel: true,
        slidesPerView: "auto",
        spaceBetween: 75,
        loop: true,
        observer:true,
			  observeParents:true,
        breakpoints: {
          1023: {
            slidesPerView: "auto",
            // centeredSlides: false,
            spaceBetween: 75,
          },
          1022: {
            slidesPerView: "auto",
            spaceBetween: 75,
          },
          320: {
            slidesPerView: 1,
            spaceBetween: 0,
          },
        },
        on: {
          resize: () => {
            setTimeout(()=> {
              this.$router.push('/blank')
            }, 500)
          },
        }
      },
      //  桌面版一個、兩個，沒有 loop
      swiperOption2: {
        // scrollbar: true,
        // mousewheel: true,
        slidesPerView: "auto",
        spaceBetween: 75,
        observer:true,
			  observeParents:true,
        on: {
          resize: () => {
            setTimeout(()=> {
              this.$router.push('/blank')
            }, 500)
          },
        }
      },
    }
  },
  mounted () {
    this.currentWidth = screen.width
    this.mySwiper.on('slideChange', () => {
      
    })

  },
  computed: {
    mySwiper () { return this.$refs.mySwiper.$swiper }
  },
  methods: {
    prevSlide() {
      // this.mySwiper.slideTo(this.slide.current - 1)
      this.mySwiper.slidePrev()
    },
    nextSlide() {
      // 桌面版 & 三個(以上)的做法
      if(this.mySwiper.realIndex == this.frames.length - 1 && this.currentWidth > 1023) {
        this.mySwiper.slideTo(0)
      } else {
        this.mySwiper.slideNext()
      }

      // this.mySwiper.slideTo(this.slide.current + 1)
      
    },
    
  },
  watch: {

  }
}
</script>

<style lang="scss">

.school {
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

  &-swiper-box {
    position: relative;
  }

  &-swiper {
    width: 100%;

    &-outer-box {
      position: relative;
      padding-top: 10px;
    }

    &-slide {
      width: 404px;
    }

    &-bg {
      background-image: url('../assets/img/school/photo-bg.png');
      background-repeat: no-repeat;
      background-size: cover;
      background-position-x: center;
      background-position-y: center;
      width: 404px;
      height: 448px;
    }

    &-box {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 44px 0px 0px 0px;
      font-weight: 500;
    }

    &-img {
      width: 283px;
      height: 283px;
      background-repeat: no-repeat;
      background-size: cover;
      background-position-x: center;
      background-position-y: center;
    }

    &-title {
      width: 283px;
      font-size: 24px;
      margin-top: 6px;
      color: black;
    }

    &-desc {
      width: 283px;
      font-size: 18px;
      margin-top: 0px;
      color: black;
    }

    &-prev {
      width: 40px;
      height: 40px;
      position: absolute;
      left: -40px;
      top: 50%;
      z-index: 1;
      cursor: pointer;

      &:hover {
        opacity: 0.8;
      }
    }

    &-next {
      width: 40px;
      height: 40px;
      position: absolute;
      right: -40px;
      top: 50%;
      z-index: 1;
      cursor: pointer;

      &:hover {
        opacity: 0.8;
      }
    }
  }

}

@media( max-width: 1023px ){

  .school {
    background-image: url('../assets/img/school/bg-m.jpg');
  

  &-outer {
    width: calc(100% - 10px);
    padding: 0px 5px;
  }

  &-title {
    flex-wrap: wrap;
    align-items: center;
    margin: 60px 0px 0px;
    font-size: 30px;

    & div:first-child {
      width: 100%;
      text-align: center;
      margin-right: 0px;
    }

    & div:nth-child(2) {
      margin-right: 10px;
    }
  }

  &-swiper-box {

  }

  &-swiper {

    &-outer-box {
      padding-top: 25px;
    }

    &-slide {
      
    }

    &-bg {
      margin: auto;
      width: 300px;
      height: 320px;
    }

    &-box {
      padding: 25px 0px 0px 0px;
    }

    &-img {
      width: 210px;
      height: 210px;
    }

    &-title {
      width: 210px;
      font-size: 18px;
    }

    &-desc {
      width: 210px;
      font-size: 16px;
    }


    &-prev {
      left: calc(50% - 162px);
      width: 30px;
      height: 30px;
    }

    &-next {
      right: calc(50% - 160px);
      width: 30px;
      height: 30px;
    }
  }

  

}

}

</style>