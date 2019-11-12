<template>

  <div id="app">
    <NavBar></NavBar>
      <div class="login_bg">
        <router-view/>
      </div>
  </div>
</template>

<script>
import Login from './components/Login.vue'
import NavBar from './components/NavBar.vue'

export default {
  name: 'app',
  components: {
    Login,
    NavBar
  }
}
</script>

<style>
.login{
  boarder: 100px 100px 100px 0px;
  text-align: center;
  padding: 100px 0px 0px 0px;


}
.login_bg{
  background-color: #0d47a1;
  background-image: -webkit-linear-gradient(100deg, #34ADFF 50%, #2196f3 50%);
  min-height: 1000px;
  padding: 0px 0px 500px 0px;

}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #34ADFF;

}
#background {
    position: fixed;
    top: 0;
    left: 0;
    width: 50%;
    height: 100%;
}
header, footer{
  background-color:#42a5f5;
  min-height: 40px;
}
nav{
  background-color:#42a5f5;
  min-height: 40px;
}
</style>
