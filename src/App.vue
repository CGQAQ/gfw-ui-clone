<template>
  <div id="app">
    <SideBar></SideBar>
  </div>
</template>

<script>
import SideBar from "./components/SideBar";

export default {
  name: 'App',
  components: {SideBar}
}
</script>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: sans-serif;
  }

  #app {
    min-width: 1065px;
    min-height: 710px;
  }

</style>
