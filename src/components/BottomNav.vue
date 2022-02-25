<template>

  <v-bottom-navigation
    app
    fixed
    grow
    v-model="activeItem"
    color="primary"
  >
    <v-btn value="code" :to="{ path: '/'}">
      <span>Home</span>
      <v-icon>home</v-icon>
    </v-btn>

    <v-btn value="top">
      <span>Share</span>
      <v-icon>share</v-icon>
    </v-btn>

  </v-bottom-navigation>

</template>

<script lang="ts">
  import { Component, Vue } from 'vue-property-decorator';
  @Component
  export default class BottomNav extends Vue {
    activeItem = 'top';
  }
</script>