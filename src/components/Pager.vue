<template>
  <div class="Pager-container">
    <a href="" class="disabled">|&lt;&lt;</a>
    <a href="">&lt;&lt;</a>
    <a href="">1</a>
    <a href="" class="active">1</a>
    <a href="">1</a>
    <a href="">1</a>
    <a href="">1</a>
    <a href="">1</a>
    <a href="">1</a>
    <a href="">&gt;&gt;</a>
    <a href="">&gt;&gt;|</a>

  </div>
</template>

<script>
//在脚本中 @ 代表src目录 
export default {

}
</script>

<style scoped lang="less">
//在样式中 ~@ 表示src目录
@import "~@/styles/var.less";
.Pager-container{
    display: flex;
    justify-content: center;  //水平居中
    margin: 20px 0;
    a{
        color: @primary;
        margin: 0 6px;
        &.disabled{
            color: @lightwords;
            cursor: not-allowed;
        }
        &.active{
            color: @words;
            font-weight:bold;  //字体加粗
            cursor:text;
        }
    }
}
</style>