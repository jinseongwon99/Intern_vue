<template>
  <div>
    <h1>Hello Vue js</h1>
    <h1>{{msg}}</h1>
    <p :title="msg">타이틀이 보입니다</p> 
    <input type="text" v-model="seen">
    <p v-if = "seen == 'test' ">if가 보입니다</p> 
    <p v-else-if = "seen == 'test1'">else if가 보입니다</p> 
    <p v-else>else가 보입니다</p> 
  </div>
</template>

<script>
export default {
  name: 'HelloVue',
  data() {
    return {
      msg: "vue Hello js"
      ,seen : 'test' 
    };
  }
}
</script>