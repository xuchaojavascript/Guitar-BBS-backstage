<template>
  <div>
    <input type="text" v-model="data.data.b">
    <button @click="viewData">查看数据</button>
  </div>
</template>
<script>
export default {
  data () {
    return {
      data: {
        data: {
          b: ''
        }
      },
      date: {}
    }
  },
  methods: {
    viewData () {
      console.log(this.data)
      console.log(this.date)
    }
  },
  mounted () {
    var a = {
      b: 12
    }
    this.data = {
      data: a
    }
    this.date = {
      data: a
    }
  }
}
</script>
<style lang="scss" scoped>
</style>
