<template>
  <div id="app" class="flex flex-col h-screen min-h-screen">
    <Header />
    <main class="relative flex-grow">
      <transition name="fade">
        <router-view />
      </transition>
    </main>
    <Footer />
  </div>
</template>
<script>
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Footer
  }
};
</script>

<style src="./assets/styles/tailwind.css"></style>
<style src="./assets/styles/main.css"></style>
