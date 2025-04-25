<script setup>
import { useRouter } from "vue-router";

const router = useRouter();
</script>

<template>
  <!-- About 3 Section -->
  <section id="about-3" class="about-3 section">

    <div class="container section-title" data-aos="fade-up">
      <h2>About Us</h2>
    </div><!-- End Section Title -->

    <div class="container">
      <div class="row gy-4 justify-content-between align-items-center">
        <div class="col-lg-6 order-lg-2 position-relative" data-aos="zoom-out">
          <img src="/img/home/home2.webp" alt="Image" class="img-fluid">
          <!--              <a href="https://www.youtube.com/watch?v=Y7f98aduVJ8" class="glightbox pulsating-play-btn">-->
          <!--                <span class="play"><i class="bi bi-play-fill"></i></span>-->
          <!--              </a>-->
        </div>
        <div class="col-lg-5 order-lg-1" data-aos="fade-up" data-aos-delay="100">
          <h2 class="content-title mb-4">Agriculture Makes Life Better</h2>
          <p class="mb-4">
            Welcome to <b>Agro Partners GH</b>, where innovative agricultural solutions
            meet trusted expertise. Our mission is to empower farmers and
            agribusinesses through sustainable practices, cutting-edge
            techniques, and unparalleled support. With years of experience
            and a commitment to eco-friendly farming, we are your partners in
            achieving maximum yields and fostering long-term growth.
          </p>
          <p>
            Our dedicated team combines deep industry knowledge with a passion
            for agriculture, ensuring that every partnership is tailored to
            your unique needs. Join us in cultivating a better future,
            one harvest at a time.
          </p>
          <ul class="list-unstyled list-check">
            <li>Leading-edge methods for better yields.</li>
            <li>Dedicated to sustainable farming solutions.</li>
            <li>Unwavering guidance from agricultural professionals.</li>
          </ul>

          <p><a class="btn-cta" @click="router.push({name: 'contact'})"
                style="cursor: pointer;"
          >Get in touch</a></p>
        </div>
      </div>
    </div>
  </section><!-- /About 3 Section -->


</template>

