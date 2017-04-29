<template>
  <div class="xin container">
     <div class="xin flex">
       <!--定义一列-->
       <div class="xin row">
         <div class="flex item">a1</div>
         <div class="flex item">a2</div>
         <div class="flex item">a3</div>
         <div class="flex item">a4</div>
       </div>
       <!--第二列-->
       <div class="xin row">
         <div class="flex item">a5</div>
         <div class="flex item">a6</div>
         <div class="flex item">a7</div>
         <div class="flex item">a8</div>
       </div>
       <!--第三列-->
        <div class="xin row">
          <div class="flex item">a9</div>
          <div class="flex item">a9</div>
        </div>
     </div>
  </div>
</template>

<script>
  export default {
    data () {
      return {}
    }
  }
</script>

<style scoped>
  .xin.container {
    width: 100%;
    padding-top: 1rem;
  }
  /*定义flex布局*/
  .xin.flex {
    display: flex;
    flex-direction: column;
  }
  /*定义每列的样式*/
  .xin.row {
    display: flex;
    flex-direction: row;
  }
  .xin.row + .xin.row {
    margin-top: 1rem;
  }
    /*定义flex布局item的默认大小*/
  .xin.flex > .flex.item, .xin.flex .flex.item {
    width: 48px;
    height: 48px;
    background-color: #0d71bb;
    text-align: center;
    line-height: 48px;
  }
  /*每列的flex row 默认是4个item*/
  .flex.item {
    margin: 0 calc((100% - 192px)/8)
  }
</style>
