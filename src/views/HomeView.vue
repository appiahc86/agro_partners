<script setup>
import {onMounted} from "vue";
import {useRouter} from "vue-router";
import ServicesComponent from "@/components/ServicesComponent.vue";
import TestimonialComponent from "@/components/TestimonialComponent.vue";
import AboutComponent from "@/components/AboutComponent.vue";

const router = useRouter();

onMounted(() => {
  const myCarouselElement = document.querySelector('#hero-carousel')
  const carousel = new bootstrap.Carousel(myCarouselElement, {
    interval: 4000,
    wrap: true,
    pause: false
  })
  carousel.cycle();


  document.querySelectorAll('.carousel-indicators').forEach((carouselIndicator) => {
    carouselIndicator.closest('.carousel').querySelectorAll('.carousel-item').forEach((carouselItem, index) => {
      if (index === 0) {
        carouselIndicator.innerHTML += `<li data-bs-target="#${carouselIndicator.closest('.carousel').id}" data-bs-slide-to="${index}" class="active"></li>`;
      } else {
        carouselIndicator.innerHTML += `<li data-bs-target="#${carouselIndicator.closest('.carousel').id}" data-bs-slide-to="${index}"></li>`;
      }
    });
  });

})

</script>

<template>
    <main class="main">

      <!-- Hero Section -->
      <section id="hero" class="hero section dark-background">

        <div id="hero-carousel" class="carousel slide carousel-fade" data-bs-ride="carousel"  data-bs-interval="4000">


          <div class="carousel-item active">
            <img src="/img/c1.jpeg" alt="">
            <div class="carousel-container">
              <h2>Building Strong Agricultural Partnerships for Growth</h2>
              <p>
                We believe in the power of collaboration, working closely with
                farmers and businesses to create mutually beneficial, thriving partnerships.
              </p>
            </div>
          </div><!-- End Carousel Item -->

          <div class="carousel-item">
            <img src="/img/c2.jpg" alt="">
            <div class="carousel-container">
              <h2>Innovating Sustainable Farming Practices for the Future</h2>
              <p>
                Our commitment to sustainability drives us to implement innovative
                farming techniques that protect the environment and ensure long-term growth.
              </p>
            </div>
          </div><!-- End Carousel Item -->

          <div class="carousel-item">
            <img src="/img/c3.jpg" alt="">
            <div class="carousel-container">
              <h2>Committed to Quality and Freshness in Every Harvest</h2>
              <p>
                Our dedication to quality ensures that every harvest is picked at its peak,
                delivering freshness and flavor with every bite.
              </p>
            </div>
          </div><!-- End Carousel Item -->

          <div class="carousel-item">
            <img src="/img/c4.jpg" alt="">
            <div class="carousel-container">
              <h2>Delivering Fresh, Locally-Sourced Produce Year-Round</h2>
              <p>
                We provide fresh, locally-sourced produce throughout the year, ensuring top-quality
                ingredients for your table every season.
              </p>
            </div>
          </div><!-- End Carousel Item -->


          <a class="carousel-control-prev" href="#hero-carousel" role="button" data-bs-slide="prev">
            <span class="carousel-control-prev-icon bi bi-chevron-left" aria-hidden="true"></span>
          </a>

          <a class="carousel-control-next" href="#hero-carousel" role="button" data-bs-slide="next">
            <span class="carousel-control-next-icon bi bi-chevron-right" aria-hidden="true"></span>
          </a>

          <ol class="carousel-indicators"></ol>


        </div>


      </section><!-- /Hero Section -->


      <ServicesComponent />


      <!-- About Section -->
      <section id="about" class="about section">

        <div class="content">
          <div class="container">
            <div class="row">
              <div class="col-lg-6 mb-4 mb-lg-0">
                <img src="/img/home/home1.webp" alt="Image " class="img-fluid img-overlap" data-aos="zoom-out">
              </div>
              <div class="col-lg-5 ml-auto" data-aos="fade-up" data-aos-delay="100">
                <h3 class="content-subtitle text-white opacity-50">Why Choose Us</h3>
                <h2 class="content-title mb-4">
                  More than <strong>50 year experience</strong> in agriculture
                  industry
                </h2>
                <p class="opacity-50">
                  Partner with us for trusted agricultural expertise,
                  innovative solutions, and a commitment to sustainable farming success.
                </p>

                <div class="row my-5">
                  <div class="col-lg-12 d-flex align-items-start mb-4">
                    <i class="bi bi-feather me-4 display-6"></i>
                    <div>
                      <h4 class="m-0 h5 text-white">Expertise in Agricultural Partnerships</h4>
                      <p class="text-white opacity-50">Proven track record of successful partnerships.</p>
                    </div>
                  </div>
                  <div class="col-lg-12 d-flex align-items-start mb-4">
                    <i class="bi bi-graph-up-arrow me-4 display-6"></i>
                    <div>
                      <h4 class="m-0 h5 text-white">Innovative Solutions</h4>
                      <p class="text-white opacity-50">Cutting-edge techniques for maximum yield.</p>
                    </div>
                  </div>
                  <div class="col-lg-12 d-flex align-items-start">
                    <i class="bi bi-people me-4 display-6"></i>
                    <div>
                      <h4 class="m-0 h5 text-white">Commitment to Sustainability</h4>
                      <p class="text-white opacity-50">Prioritizing eco-friendly farming practices always.</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section><!-- /About Section -->


      <AboutComponent />

      <!-- Testimonials Section -->
<TestimonialComponent />

    </main>

</template>
