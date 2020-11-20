<template>
  <div id="app">
    <change/>
    <Jia></Jia>
    <hello-world msg="Welcome to Your Vue.js App"/>
    <Icon class="icon"></Icon>
    <Button></Button>
    <built-in></built-in>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Icon from "@/components/Icon";
import Button from "@/components/Button";
import Jia from "@/components/Jia";
import Change from "@/components/Change";
import BuiltIn from "@/components/BuiltIn";
export default {
  name: 'app',
  components: {
    BuiltIn,
    HelloWorld,
    Icon,
    Button,
    Jia,
    Change
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.icon{
  padding-top: 10px;
}
</style>
