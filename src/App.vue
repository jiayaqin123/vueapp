<template>
  <div id="app">
    <div class="nav">
      <div class="nav1"></div>
      Sous
      <div class="nav2"></div>
    </div>
    <AppMenu></AppMenu>
    <InputBar></InputBar>
    <ListBox></ListBox>
  </div>
</template>

<script>
import AppMenu from './components/Menu'
import InputBar from './components/InputBar'
import ListBox from './components/ListBox'
export default {
  name: 'app',
  components: {
    AppMenu,
    InputBar,
    ListBox
  }
}
</script>

<style>

#app {

}
.nav{
  width:100%;
  height:0.6rem;
  background:#333;
  color:#fff;
  text-align:center;
  line-height:0.6rem;
}
</style>
