<template>
  <div id="app">
    <PropsVue myData1="This is for HOME PAGE"/>
    <PropsVue myData2="This is for PRODUCT PAGE" samData="hello sam !!!"/>
    <ifElse/>
    <elseIf/> 
    <ternoryOperator/>
    <ForInObj/>
    <ForInArray/>
    <ForInLoop/>
    <vOnce/>
    <vBind/>
  </div>
</template>

<script>
import PropsVue from './components/PropsVue.vue'
import IfElse from './components/IfElse.vue'
import elseIf from './components/elseIf.vue'
import ForInObj from './components/ForInObj.vue'
import ForInArray from './components/ForInArray.vue'
import ForInLoop from './components/ForInLoop.vue'
import vOnce from './components/vOnce.vue'
import ternoryOperator from './components/ternoryOperator.vue'
import vBind from './components/vBind.vue'

export default {
  name: 'App',
  components: {
    PropsVue,
    IfElse,
    elseIf,
    ForInObj,
    ForInArray,
    ForInLoop,
    vOnce,
    ternoryOperator,
    vBind
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
