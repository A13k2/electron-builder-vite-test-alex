<script lang="ts" setup>
import ElectronVersions from '/@/components/ElectronVersions.vue';
import ReactiveHash from '/@/components/ReactiveHash.vue';

const APP_VERSION = import.meta.env.VITE_APP_VERSION;
</script>

<template>
  <img
    alt="Vue logo"
    src="../assets/logo.svg"
    width="150"
  />

  <p>
    <!-- Example how to inject current app version to UI -->
    App version: {{ APP_VERSION }}
  </p>

  <p>
    New version auto updater testing 🚀
  </p>


  <fieldset>
    <legend>Test Node.js API</legend>
    <reactive-hash />
  </fieldset>

  <fieldset>
    <legend>Environment</legend>
    <electron-versions />
  </fieldset>

  <p>
    Edit
    <code>packages/renderer/src/App.vue</code> to test hot module replacement.
  </p>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 60px auto;
  max-width: 700px;
}

fieldset {
  margin: 2rem;
  padding: 1rem;
}
</style>
