<template>
    <v-app-bar height="50" color="black" density="compact" flat>
        <template v-slot:prepend>
            <span class="mdi mdi-map-marker">
            </span>
        </template>

        <v-app-bar-title class="v-app-bar">Deira ,baniyas st, twin towers 22d floor, inox bussines center ,unit no:9 </v-app-bar-title>

        <template v-slot:append>
            <v-btn color="green" flat class="mdi mdi-twitter"></v-btn>
            <v-btn color="green" flat class="mdi mdi-whatsapp"></v-btn>
            <v-btn color="green" flat class="mdi mdi-facebook"></v-btn>
        </template>
    </v-app-bar>
    <custom-navbar></custom-navbar>
</template>
<script setup lang="ts">
import CustomNavbar from "@/components/CustomNavbar.vue"
</script>
<style scoped>
.v-app-bar{
    font-size: 15px !important;
}
</style>