<template>
  <v-app>
    <TopToolbar />
    <v-main>
      <router-view />
    </v-main>
    <BottomNav />
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import TopToolbar from "./components/TopToolbar.vue";
import BottomNav from "./components/BottomNav.vue";
import HelloWorld from "./components/HelloWorld.vue";
import About from "./views/About.vue";
@Component({
  components: {
    TopToolbar,
    BottomNav,
    HelloWorld,
    About,
  },
})
export default class extends Vue {}
</script>