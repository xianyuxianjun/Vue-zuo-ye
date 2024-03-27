<template>
  <div class="app">
<!--    <One></One>-->
<!--    <Tow></Tow>-->
<!--    <Three></Three>-->
<!--    <Four></Four>-->
<!--    <Five></Five>-->
<!--    <P66 v-if="zu==1"></P66>-->
    <P67 v-if="zu==1
























"></P67>
    <button @click="xiaohui">点我销毁组件,再次点击生成组件</button>

  </div>
</template>

<script setup>
  import One from "@/day01/One.vue";
  import Tow from "@/day01/Three.vue";
  import Four from "@/day01/Four.vue";
  import Three from "@/day01/Three.vue";
  import Five from "@/day01/Five.vue";
  import P66 from "@/day02/P66.vue";
  import {ref} from "vue";
  import P67 from "@/day02/P67.vue";
  let zu=ref(1)
  function xiaohui(){
    if (zu.value==1){
      zu.value=0
    }else{
      zu.value=1
    }
  }
</script>

<style scoped>
.app {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
