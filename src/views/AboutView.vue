<script setup>
import { RouterLink } from "vue-router"
import { useRouter } from "vue-router";

const router = useRouter();

import ServicesComponent from "@/components/ServicesComponent.vue";
import AboutComponent from "@/components/AboutComponent.vue";
</script>
<template>
  <main class="main">

    <!-- Page Title -->
    <div class="page-title dark-background" data-aos="fade" style="background-image: url(/img/page-title-bg.webp);">
      <div class="container position-relative">
        <h1>About Us</h1>
        <p>We are dedicated to fostering strong agricultural partnerships,
          providing innovative solutions, and supporting sustainable growth in farming.</p>
        <nav class="breadcrumbs">
          <ol>
            <li><router-link :to="{name: 'home'}">Home</router-link></li>
            <li class="current">About</li>
          </ol>
        </nav>
      </div>
    </div><!-- End Page Title -->

    <!-- About 3 Section -->
  <AboutComponent />
    <!-- Team Section -->
    <section class="team-15 team section" id="team">
      <!-- Section Title -->
      <div class="container section-title" data-aos="fade-up">
        <h2>Team</h2>
        <p>Dedicated experts in innovative and sustainable agriculture.</p>
      </div><!-- End Section Title -->

      <div class="content">
        <div class="container">

          <div class="row">
            <div class="col-lg-3 col-md-6 mb-4">
              <div class="person">
                <figure>
                  <img src="/img/team/samuel.jpg" alt="Image" class="img-fluid w-100">
                  <div class="social">
                    <a href="#"><span class="bi bi-facebook"></span></a>
                    <a href="#"><span class="bi bi-twitter-x"></span></a>
                    <a href="#"><span class="bi bi-linkedin"></span></a>
                  </div>
                </figure>
                <div class="person-contents">
                  <h3>Mr. Samuel Amissah</h3>
                  <span class="position">CEO</span>
                </div>
              </div>
            </div>

            <div class="col-lg-3 col-md-6 mb-4">
              <div class="person">
                <figure>
                  <img src="/img/team/sebe.jpg" alt="Image" class="img-fluid w-100">
                  <div class="social">
                    <a href="#"><span class="bi bi-facebook"></span></a>
                    <a href="#"><span class="bi bi-twitter-x"></span></a>
                    <a href="#"><span class="bi bi-linkedin"></span></a>
                  </div>
                </figure>
                <div class="person-contents">
                  <h3>Mr. Kofi Sebe</h3>
                  <span class="position">General Manager</span>
                </div>
              </div>
            </div>

            <div class="col-lg-3 col-md-6 mb-4">
              <div class="person">
                <figure>
                  <img src="/img/team/ellen.jpg" alt="Image" class="img-fluid w-100">
                  <div class="social">
                    <a href="#"><span class="bi bi-facebook"></span></a>
                    <a href="#"><span class="bi bi-twitter-x"></span></a>
                    <a href="#"><span class="bi bi-linkedin"></span></a>
                  </div>
                </figure>
                <div class="person-contents">
                  <h3>Ms Ellen Addai</h3>
                  <span class="position">Project Administrator</span>
                </div>
              </div>
            </div>

            <div class="col-lg-3 col-md-6 mb-4">
              <div class="person">
                <figure>
                  <img src="/img/team/constance.jpeg" alt="Image" class="img-fluid w-100">
                  <div class="social">
                    <a href="#"><span class="bi bi-facebook"></span></a>
                    <a href="#"><span class="bi bi-twitter-x"></span></a>
                    <a href="#"><span class="bi bi-linkedin"></span></a>
                  </div>
                </figure>
                <div class="person-contents">
                  <h3>Mrs Constance Opoku</h3>
                  <span class="position">Sales & Marketing</span>
                </div>
              </div>
            </div>

          </div>
        </div>
      </div>

    </section><!-- /Team Section -->


    <ServicesComponent />

  </main>
</template>

<style>

</style>
