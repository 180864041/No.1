<template>
  <i class="iconfont" :class="fontClass"></i>
</template>

<script>
//样式映射
const classMap = {
    home:"icon-home",
    success:"icon-success",
    error:"icon-error",
    close:"icon-close",
    warn:"icon-warn",
    info:"icon-info",
    blog:"icon-wenzhang",
    code:"icon-code",
    about:"icon-guanyuwo",
    weixin:"icon-weixin",
    qq:"icon-QQ",
    mail:"icon-youxiang",
    github:"icon-github-fill",
    arrowUp:"icon-arrow-up-bold",
    arrowDown:"icon-arrow-down",
    empty:"icon-empty",
    message:"icon-liuyanban"
}
export default {
props:{
    type:{
        type:String,
        require:true,
    }
},
computed:{
    //图标样式
    fontClass(){
        return classMap[this.type]
    }
}
}
</script>

<style scoped>
@import "//at.alicdn.com/t/c/font_3273192_n1ijmub56kl.css";
</style>>

</style>