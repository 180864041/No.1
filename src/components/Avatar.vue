<template>
  <img
  class="Avatar-container" 
  :src="url" 
  :style="{
    width:size + 'px',
    height:size + 'px'
  }">
</template>

<script>
export default {
props:{
    url:{
        type:String,
        require:true,
    },
   size:{
        type:Number,
        default:50
    },
  
}
}
</script>

<style scoped>
.Avatar-container{
    border-radius: 50%;
    object-fit: cover;  /* 适应指定容器的高度与宽度。 */
    display: block;
}
</style>