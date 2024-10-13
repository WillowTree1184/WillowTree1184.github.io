<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Lenis from 'lenis'

const lenis = new Lenis();

lenis.on('scroll', (e) => {
  console.log(e);
});

function raf(time) {
  lenis.raf(time * 1.5);
  requestAnimationFrame(raf);
}

requestAnimationFrame(raf);

</script>

<template>
  <RouterView />
</template>