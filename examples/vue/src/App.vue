<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import Header from './components/Header.vue';
import Icons from './components/Icons.vue';
import Meta2d from './components/Meta2d.vue';
</script>

<template>
  <Header />
  <Icons />
  <Meta2d />
</template>

<style>
* {
  padding: 0;
  margin: 0;
  outline: none;
  box-sizing: border-box;
  word-break: break-all;
  word-break: break-word;
}

html, body, #app {
  width: 100%;
  height: 100%;
}

input[type=file], /* FF, IE7+, chrome (except button) */
input[type=file]::-webkit-file-upload-button { /* chromes and blink button */
  cursor: pointer; 
}

i.iconfont {
  font-size: 30px;
  color: rgba(0,0,0,.65);
}

.header {
  height: 61px;
  border-bottom: 1px solid #ccc;
}

.logo, .button-group {
  height: 60px;
}

.logo {
  width: 100px;
  padding: 5px;
  float: left;
  text-align: center;
}

.logo img {
  width: 50px;
  height: 50px;
}

.button-group {
  text-align: center;
  padding: 14px;
  padding-left: 100px;
}

.button-group button {
  width: 100px;
  height: 32px;
  border: 1px solid #1890ff;
  border-radius: 2px;
  color: #1890ff;
  background-color: transparent;
  cursor: pointer;
}

.button-group button:hover,
.button-group button.active {
  background-color: #1890ff;
  color: #fff;
}

.button-group > button + button {
  margin-left: 10px;
}

#open {
  position: relative;
}

#open-input {
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  opacity: 0;
}

.aside {
  width: 101px;
  height: calc(100% - 61px);
  float: left;
  border-right: 1px solid #ccc;
  background-color: #fff;
}

.aside .icon-list {
  border-bottom: 1px solid #ccc;
}

.aside .icon-list > div,
.aside .link {
  height: 51px;
  line-height: 50px;
  text-align: center;
}

.aside .icon-list > div i {
  cursor: pointer;
  user-select: none;
}

.main {
  height: calc(100% - 61px);
  padding-left: 101px;
}

#meta2d {
  height: 100%;
}
</style>
