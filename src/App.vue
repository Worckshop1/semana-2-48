<template>
  <div id="app">
    <div class="container-fluid">
      <module-api></module-api>
    </div>
  </div>
</template>

<script>
import ModuleApi from "./components/ModuleApi.vue";

export default {
  name: "App",
  components: {
    ModuleApi,
  },
};
</script>

