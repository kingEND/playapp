<template>
  <div id="container">
    <div id="scroll">
      <div class="article">
        <img src="../assets/logo.png" alt="无法显示">
        <h1>Duis volutpat</h1>
        <p>phasellus hendrerit .. vitae viverra nisl.</p>
      </div>
      <div class="article">
        <img src="../assets/logo.png" alt="无法显示">
        <h1>Duis volutpat</h1>
        <p>phasellus hendrerit .. vitae viverra nisl.</p>
      </div>
      <div class="article">
        <img src="../assets/logo.png" alt="无法显示">
        <h1>Duis volutpat</h1>
        <p>phasellus hendrerit .. vitae viverra nisl.</p>
      </div>
    </div>
    {{message}}
    {{msg}}
    <button @click="updataMessage">更新</button>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        message: 'not Update',
        msg: 'sucessful'
      }
    },
    methods: {
      updataMessage () {
        this.message = 'update'
        this.msg = 'set'
        console.log(this.$el.textContent)
//        this.$nextTick(function () {
//          console.log(this.$el.textContent)
//        })
      }
    }
  }
</script>

<style scoped>
</style>
