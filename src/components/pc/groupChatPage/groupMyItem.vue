<template>
  <div style="float:right; width:100%; margin-bottom:0.1rem">
    <img :src="img" alt="头像" style="float:right;width: 0.5rem;height: 0.5rem;">
    <div v-if="messageid === 0" style="display:inline-block; font-size:0.4rem;margin-right:0.2rem;max-width:50%;word-wrap:break-word;word-break:break-all;float:inherit;text-align:left">{{msg}}</div>
    <img v-if="messageid === 1" :src="msg" alt="图片加载失败" style="display:inline-block; margin-right:0.2rem;max-width:50%;word-wrap:break-word;word-break:break-all;float:inherit;text-align:left"/>
  </div>
</template>

<script>
export default {
  name: 'my-item',
  props: ["messageid", 'me', 'name', 'img', 'msg'], 
}
</script>

<style>

</style>