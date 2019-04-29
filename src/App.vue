<template>
  <div id="app">
    <Chat/>
    <vue-webrtc width="100%" roomId="roomId"></vue-webrtc>
  </div>
</template>

<script>
import Vue from "vue";
import WebRTC from "vue-webrtc";

import Chat from "./components/Chat";

Vue.use(WebRTC);

export default {
  name: "App",
  components: {
    Chat
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
