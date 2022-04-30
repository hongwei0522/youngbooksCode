<template>
  <div>
    <!-- <topBar/> -->
    <div class="default-setting">
      <nuxt/>
    </div>
    
    <!-- <bottomBar/> -->
  </div>
</template>

<script>

export default {
  components: {
    topBar: require('~/components/top-bar.vue').default,
    bottomBar: require('~/components/bottom-bar.vue').default
  },
  props: {

  },
  data () {
    return {
      
    }
  },
  mounted () {
    
  },
  computed: {

  },
  methods: {

  },
  watch: {
    '$route.name': {
      handler: function(name) {
        
      },
      immediate: true
    }
  }
}
</script>

<style lang="scss">

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
  line-height: 1.5;
  letter-spacing: 0.1em;
	vertical-align: baseline;
  scroll-behavior: smooth;
}

/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display: block;
}

ol, ul {
	list-style: none;
}

blockquote, q {
	quotes: none;
}

blockquote:before, blockquote:after,
q:before, q:after {
	content: '';
	content: none;
}

table {
	border-collapse: collapse;
	border-spacing: 0;
}

body {
  margin: 0px;
  padding: 0px;
  font-family: 'NotoSansTC', 'Roboto', 'Noto Sans TC', 'Noto Sans SC' ,sans-serif;
  font-size: 18px;
  font-weight: 300;
  // color: #FFFFFF;
  // background-color: #171719;
}

a {
  color: #fff;
  text-decoration: none;
}

input {
  padding: 0px;
  margin: 0px;
  outline: none;
 -webkit-appearance: none;
 -webkit-tap-highlight-color: rgba(0, 0, 0, 0);

  &:focus {
    outline: none;
  }

  &::placeholder {
    color: rgba(0, 0, 0, 0.6);
  }
}

textarea {

  &:focus {
    outline: none;
  }

  &::placeholder {
    color: rgba(0, 0, 0, 0.6);
  }
}

.default-setting {
  
}

@media( max-width: 1023px ){

  body {
    font-size: 14px;
  }

}

</style>
