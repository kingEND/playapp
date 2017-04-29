<template>
  <div>
    <tabs  top="true"></tabs>
    <router-view></router-view>
    <tabs tabsclass="bottom"></tabs>
  </div>
</template>

<script>
  import tabs from './components/common/tabs.vue'
  export default {
    name: 'app',
    components: {tabs}
  }
</script>

<style>
  @import "assets/css/dist/semantic.css";
  @import "assets/css/base.css";
</style>
