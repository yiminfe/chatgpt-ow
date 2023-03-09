<template>
  <div class="app">
    <Navbar />
    <Header />
    <Features />
    <UseCases />
    <Footer />
  </div>
</template>

<script setup>
import Navbar from '@/components/Navbar.vue'
import Header from '@/components/Header.vue'
import Features from '@/components/Features.vue'
import UseCases from '@/components/UseCases.vue'
import Footer from '@/components/Footer.vue'
</script>

<style>
.app {
  font-family: 'Helvetica Neue', sans-serif;
}
</style>
