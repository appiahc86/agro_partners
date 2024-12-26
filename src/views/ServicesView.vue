<script setup>
import { RouterLink } from "vue-router";
import TestimonialComponent from "@/components/TestimonialComponent.vue";
import ServicesComponent from "@/components/ServicesComponent.vue";
</script>

<template>
  <main class="main">

    <!-- Page Title -->
    <div class="page-title dark-background" data-aos="fade" style="background-image: url(/img/page-title-bg.webp);">
      <div class="container position-relative">
        <h1>Services</h1>
        <nav class="breadcrumbs">
          <ol>
            <li><router-link :to="{name: 'home'}">Home</router-link></li>
            <li class="current">Services</li>
          </ol>
        </nav>
      </div>
    </div><!-- End Page Title -->

    <!-- Services Section -->
<ServicesComponent />
    <TestimonialComponent />

  </main>

</template>

<style scoped>

</style>