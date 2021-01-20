<template>
  <div id="app">
    <keep-alive exclude="Detail">
      <router-view></router-view>
    </keep-alive>
    <MainTaBar></MainTaBar>
  </div>
</template>

<script>
import MainTaBar from "components/content/maintarbar/MainTarBar";
export default {
  name: "App",
  components: {
    MainTaBar,
  },
};
</script>

<style>
@import "./assets/css/base.css";
</style>
