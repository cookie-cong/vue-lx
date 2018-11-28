<template>
  <div id="app">
 <!-- 父组件 -->
    <!-- <input type="text" v-model="name"> -->
    
    <span>{{name}}</span>
    <br>
    <br>
    <one @child="child"></one>
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
  },
  methods:{
    child(valueNmae){
      this.name=valueNmae
    }
  }
}
</script>

<style>

</style>
