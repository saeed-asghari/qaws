<script setup lang="ts">
</script>

<template>
  <v-app>
    <v-main>
      <custom-header></custom-header>
      <v-container class="pa-0">
        <router-view></router-view>
      </v-container>
      <custom-footer></custom-footer>
    </v-main>
  </v-app>
</template>

<script setup lang="ts">
import CustomHeader from "@/components/CustomHeader.vue"
import CustomFooter from "@/components/CustomFooter.vue"
</script>
<style>

</style>