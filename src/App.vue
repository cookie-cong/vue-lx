<template>
  <div id="app">
 <!-- 父组件 -->
    <input type="text" v-model="name">
    <one :name="name"></one>
  </div>
</template>

<script>
import one from "./components/one"
export default {
  name: 'App',
  components:{
    one
  },
  data(){
    return{
      name:""
    }
  }
}
</script>

<style>

</style>
