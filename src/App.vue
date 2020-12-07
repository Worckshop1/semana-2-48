<template>
  <div id="app">
    <module-banner></module-banner>
    <div class="container-fluid">
      <module-api></module-api>
    </div>
    <module-footer></module-footer>
  </div>
</template>

<script>
import ModuleBanner from "./components/ModuleBanner.vue";
import ModuleApi from "./components/ModuleApi.vue";
import ModuleFooter from "./components/ModuleFooter.vue";

export default {
  name: "App",
  components: {
    ModuleApi,
    ModuleFooter,
    ModuleBanner,
  },
};
</script>

