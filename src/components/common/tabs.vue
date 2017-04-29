<template>
  <div class="xin tabs" :class="tabsclass">
    <div class="xin header" v-if="top">{{title}}</div>
    <div class="xin flex" v-else>
      <div class="flex item">我的</div>
      <div class="flex item">我的</div>
      <div class="flex item">我的</div>
      <div class="flex item">我的</div>
    </div>
  </div>
</template>

<script>
  export default {
    props: {
      title: {
        default: '私人定义'
      },
      tabsclass: {},
      top: {
        default: false
      }
    },
    data () {
      return {}
    }
  }
</script>

<style scoped>
  /*定义主页面的tabs*/
  .xin.tabs {
    width: 100%;
    height: 48px;
    line-height: 48px;
    text-align: center;
    font-size: 16px;
    background-color: #00b5ad;
    color: black;
    font-weight: bold;
  }

  .xin.tabs.bottom {
    position: fixed;
    bottom: 0;
    left: 0;
  }

  .xin.flex {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
  }

  .flex.item {
    width: 48px;
    height: 48px;
  }
</style>
