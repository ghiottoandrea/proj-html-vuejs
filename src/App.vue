<script>
import headerApp from './components/headerApp.vue';
import mainApp from './components/mainApp.vue';
import footerApp from './components/footerApp.vue';

export default {
  name: App,
  components: {
    headerApp,
    mainApp,
    footerApp,
  }
}
</script>

<template>

<headerApp />
<mainApp />
<footerApp />

</template>

<style></style>
