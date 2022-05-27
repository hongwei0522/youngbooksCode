<template>
  <div>
    <schoolContain :title="title" :frames="frames" />
  </div>
</template>

<script>

import { schoolList } from '@/assets/list/schoolList'
export default {
  head() {
    return {
      title: '閱讀私角落　校園攝影展',
      meta: [
        { charset: 'utf-8' },
        { hid: 'og:title'  , property: 'og:title'  , content: '閱讀私角落　校園攝影展' },
        { hid: 'og:image' , property: 'og:image' , content: require('@/assets/img/article/n01/1.jpg') },
        { hid: 'description', name: 'description', content: '有一個角落，可以自由呼吸 有一個角落，可以滋養閱讀。' },
        { hid: 'og:description' , property: 'og:description' , content: '有一個角落，可以自由呼吸 有一個角落，可以滋養閱讀。' },
      ],
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
      schoolList: schoolList,
      title: '',
      frames: [],
      urlName: '',
      place: ''
    }
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