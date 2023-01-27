<template>
    <v-app-bar height="48" class="bg-light" elevation="0">
        <div class="navbar-container">
            <ul>
                <li v-for="item in menu" :key="item.id" :class="item.active ? 'active' : ''"
                    @click="toggleClass(item.id)">
                    <router-link :to="item.route">{{ item.name }}</router-link>
                    <div class="underline"></div>
                </li>
            </ul>
        </div>

    
    </v-app-bar>
</template>
<script setup lang="ts">
import { ref, type Ref } from 'vue';
interface RouterMenu {
    id: number;
    name: string;
    route: string;
    active: boolean

}
const menu: Ref<RouterMenu[]> = ref([{ id: 0, name: 'Home', route: "/", active: true }, { id: 1, name: 'About', route: "/About", active: false }] as RouterMenu[])
const toggleClass = (id: number) => {
    menu.value.map((item) => {
        item.active = false
    });
    menu.value.find(a => a.id == id)!.active = !menu.value.find(a => a.id == id)!.active;

}
</script>
<style >
.bg-light {
    background-color: #f8f9fa !important
}

a {
    outline: none;
}

.navbar-container {
    text-align: center;
    background-color: #009688;
    padding: 10px;
    font-size: 0;
    width: 100%;
}

.navbar-container ul {
    margin: 0;
    padding: 0;
    text-align: right;
    display: inline-block;
    vertical-align: middle;
}

.navbar-container ul li {
    display: inline-block;
    font-size: 16px;
}

.navbar-container ul li a {
    color: #ffffff;
    text-decoration: none;
    display: inline-block;
    padding: 10px;
    transition: color 0.5s;
}

.navbar-container ul li .underline {
    height: 3px;
    background-color: transparent;
    width: 0%;
    transition: width 0.2s, background-color 0.5s;
    margin: 0 auto;
}

.active.underline ::before {
    /* content: "";
    position: absolute;
    width: 100%;
    height: 8px;
    background-color: #6A6E7B;
    bottom: 0;
    right: 0%;
    left: 0%;
    border-radius: 10px 10px 0 0; */
}

.navbar-container ul li.active .underline {
    width: 100%;
    background-color: white;
}

.navbar-container ul li:hover .underline {
    background-color: white;
    width: 100%;
}



.navbar-container ul li:active a {
    transition: none;
    color: rgba(255, 255, 255, 0.76);

}

.navbar-container ul li:active .underline {
    transition: none;
    background-color: rgba(255, 255, 255, 0.76);
}
</style>