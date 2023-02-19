<script lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Navbar from "./components/Navbar.vue";

export default {
  name: 'app',

  components: { Navbar },

  data() {
    return { top: 21 }
  },

  methods: {
    scrollToTop() {
      window.scrollTo({
        top: 0,
        behavior: "smooth",
      });
    },
    handleCreate() {
      console.log('component has been created.');
    }
  }
}
</script>

<template>
  <div class="app">
    <!-- Navbar -->
    <header>
      <Navbar @vnode-mounted="handleCreate" />
    </header>

    <!-- Dot that go back to top on click -->
    <div class="dot" @click="scrollToTop">
      <i class="ri-arrow-up-line"></i>
    </div>

    <RouterView />
  </div>
</template>

<!-- style without 'scoped' to apply to all HTML -->
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;0,400;0,500;1,200;1,300;1,400;1,500&display=swap');

* {
  margin: 0;
  padding: 0;
  border: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

:root {
  --background-color: white;
  --text-color: black;
}

.dark-mode {
  --background-color: #121212;
  --text-color: white;
}

body {
  background-color: var(--background-color);
  color: var(--text-color);
}

.dot {
  height: 50px;
  width: 50px;
  position: fixed;
  bottom: 0;
  right: 0;
  margin: 20px;
  background-color: #f7f7f7b0;
  border-radius: 50%;
  z-index: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.dot:hover {
  background-color: #f7f7f7;
  cursor: pointer;
}
</style>
