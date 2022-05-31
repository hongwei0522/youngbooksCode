<template>
  <div>
    <schoolContain :title="title" :frames="frames" />

    <schoolAnimate v-show="isShowH" :title="title" />
    <schoolAnimate2 v-show="isShowU" :title="title" />
  </div>
</template>

<script>

import { schoolList } from '@/assets/list/schoolList'
export default {
  layout: 'default',
  components: {
    schoolAnimate: require('~/components/school-animate.vue').default,
    schoolAnimate2: require('~/components/school-animate2.vue').default,
    schoolContain: require('~/components/school-contain.vue').default,
  },
  props: {
    
  },
  data () {
    return {
      schoolList: schoolList,
      title: '',
      frames: [],
      urlName: '',
      place: '',
      isShowH: false,
      isShowU: false,
      isFromInsidePage: false
    }
  },
  beforeRouteEnter(to, from, next) {
    next(vm => {
      // 判斷是否從內頁過來
      if(from.name) {
        if(from.name.substr(0, 8) == 'schoolin') {
          vm.isFromInsidePage = true
        }
      }
      vm.prevRoute = from
    })
  },
  mounted () {
    // 取得網址列參數
    // 101
    // 1 北部 2 中部 3 南部 4 東部 5 外島
    // 第一張第二張
    // 取得標題
    // 判斷高中、大學
    // 判斷北中南
    // 取得圖片
    let urlParams = new URLSearchParams(window.location.search)
    this.urlName = parseInt(urlParams.get('name'))
    this.urlName = this.urlName.toString()
    if(this.urlName.substr(0, 1) == 1) {
      this.place = 'n'
    } else if(this.urlName.substr(0, 1) == 2) {
      this.place = 'm'
    } else if(this.urlName.substr(0, 1) == 3) {
      this.place = 's'
    } else if(this.urlName.substr(0, 1) == 4) {
      this.place = 'e'
    } else if(this.urlName.substr(0, 1) == 5) {
      this.place = 'i'
    }

    // 在 component 內塞入標題與圖片
    for(let i = 0; i < this.schoolList.length; i++) {
      if(this.schoolList[i].link.substr(0, 3) == this.urlName) {
        this.title = this.schoolList[i].name
        this.frames.push(this.schoolList[i])
      }
    }

    // 動畫
    let tempUrlName = parseInt(urlParams.get('name'))
    for(let i = 0; i < this.schoolList.length; i++) {
      if(this.schoolList[i].link == tempUrlName + '01') {
        // 改 title
        this.title = this.schoolList[i].name
        // 判斷大學
        if(!this.isFromInsidePage) {
          this.showAnimate(this.schoolList[i].type)
          this.isFromInsidePage = false
        }
        
      }
    }

  },
  computed: {

  },
  methods: {
    showAnimate(type) {
      if(type == 'h') {
        this.isShowH = true
        setTimeout(() => {
          this.isShowH = false
        }, 3000)
      } else {
        this.isShowU = true
        setTimeout(() => {
          this.isShowU = false
        }, 3000)
      }
    }
  },
  watch: {
    '$route.name': {
      handler: function(name) {
        if(name == 'school') {
          // let urlParams = new URLSearchParams(window.location.search)
          // this.urlName = parseInt(urlParams.get('name'))
          // for(let i = 0; i < this.schoolList.length; i++) {
          //   if(this.schoolList[i].link == this.urlName + '01') {
          //     // 改 title
          //     this.title = this.schoolList[i].name
          //     // 判斷大學
          //     this.showAnimate(this.schoolList[i].type)
          //   }
          // }
        }
      },
      // immediate: true
    }
  }
}
</script>

<style lang="scss" scoped>

</style>