<template>
  <el-select v-model="select.current" placeholder="選擇校園">
    <el-option
      v-for="option in options"
      :key="option.name"
      :label="option.name"
      :value="option.name"
    >
    </el-option>
  </el-select>
</template>

<script>
export default {
  components: {

  },
  props: {
    options: {
      type: Array
    },
  },
  data () {
    return {
      select: {
        current: '選擇校園',
      }
    }
  },
  computed: {

  },
  methods: {

  },
  watch: {
    'select.current': {
      handler: function(data) {
        for(let j = 0; j < this.options.length; j++) {
          if(this.options[j].name == data) {
            this.$router.push('/school?name=' + this.options[j].link.substr(0,3))
          }
        }
      },
    }
  }
}
</script>

<style lang="scss">



</style>

<style>

.el-input--suffix .el-input__inner {
  width: 293px;
  color: #000000;
  background-color: #D8D76F;
  font-size: 20px;
  border: 2px solid #7C794B;
  border-radius: 20px;
}

.el-select .el-input.is-focus .el-input__inner {
  border: 2px solid #7C794B;
}

.el-select .el-input__inner:focus {
  border: 2px solid #7C794B;
}

.el-input__suffix {
  color: #000000;
}

.el-select .el-input .el-select__caret {
  color: #000000;
  font-size: 24px;
  font-weight: bold;
  margin: 2px 10px 0px 0px;
}

.el-select-dropdown__item.selected {
  color: #000000;
  font-weight: bold;
}

</style>