

<template>
  <footer>
    <div class="footer-contaner">
      <div>
        <h5>About</h5>
        <ul class="list-unstyled text-small">
          <li>
            <router-link to="/">Home</router-link>
          </li>
          <li>
            <router-link to="/">Location</router-link>
          </li>
          <li>
            <router-link to="/">Contacts</router-link>
          </li>
          <li>
            <router-link to="/">Opening Hours</router-link>
          </li>
        </ul>
      </div>

      <div>
        <h5>Join Us</h5>
        <ul class="list-unstyled text-small">
          <li>
            <router-link to="/">Twitter</router-link>
          </li>
          <li>
            <router-link to="/">Facebook</router-link>
          </li>
          <li>
            <router-link to="/">Instagram</router-link>
          </li>
          <li>
            <router-link to="/">Linkedin</router-link>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>
<script setup lang="ts">
import { ref } from "vue";

import type { Ref } from "vue";
let CurrentYear: Ref<string> = ref(new Date().getFullYear().toString());
</script>
<style  scoped>
/* footer */
.footer-contaner {
  color: #ffffff;
  background: #111111;
  padding: 40px 20px;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  justify-items: center;
  position: fixed;
  width: 100%;
  bottom: 0%;
  left: 0;
}

.footer-contaner a {
  color: #6c757d;
  text-decoration: none;
}

.footer-contaner a:hover {
  color: #ffffff;
}
</style>