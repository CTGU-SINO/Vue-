<template>
  <div id="app">
    <h1>{{title}}</h1>
    <ul>
      <li><router-link to="/">Home</router-link></li>
      <li><router-link to="/index">Index</router-link></li>
    </ul>
    <router-view></router-view>
    <app-header></app-header>
    <users></users>
    <app-footer></app-footer>
  </div>
</template>

<script>

// 局部注册
import Users from './components/Users'
import Header from './components/Header'
import Footer from './components/Footer'

export default {
  name: 'App',
  data(){
    return {
      title:"这是我的第一个vue脚手架project！"
    }
  },
  components:{
    'users':Users,
    'app-header':Header,
    'app-footer':Footer
  }
}
</script>

// 样式作用域
<style scoped>

</style>
