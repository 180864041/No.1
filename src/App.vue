<template>
  <div id="app">
   <Avatar url="https://img1.baidu.com/it/u=1511505210,3146144939&fm=253&app=138&size=w931&n=0&f=JPG&fmt=auto?sec=1660928400&t=3c8301c60b6bb8caf2b43d64b8413c5f"
   :size="100" />
   <Icon type="info" />
   <Pager />
  </div>
</template>


<script>
import Avatar from "./components/Avatar.vue"
import Icon from "./components/Icon.vue"
import Pager from "./components/Pager.vue"
export default {
  name:"App",
  components:{
    Avatar,
    Icon,
    Pager
  }
}
</script>

<style scoped>
/* 这里可以通过子组件的类样式在父组件中控制子组件的样式 */
.iconfont{
  font-size: 26px;
  color: red;
}
</style>