<script setup lang="ts">
</script>

<template>
  <v-app>
    <v-main>
      <custom-header></custom-header>
      <div class="pa-0">
        <router-view></router-view>
      </div>
      <custom-footer></custom-footer>
    </v-main>
  </v-app>
</template>

<script setup lang="ts">

import CustomHeader from "@/components/CustomHeader.vue"
import CustomFooter from "@/components/CustomFooter.vue"
import { onMounted} from 'vue';
import router from '@/router';
router:router
onMounted(()=>{
    router.push('/')
})
</script>
<style>

</style>