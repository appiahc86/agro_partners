<script setup>
import  { RouterLink } from "vue-router";
import {useRouter} from "vue-router";

const router = useRouter();
</script>/
<template>
  <header id="header" class="header d-flex align-items-center position-relative">
    <div class="container-fluid container-xl position-relative d-flex align-items-center justify-content-between">

      <a  class="logo d-flex align-items-center"
          @click="router.push({name: 'home'})"
      style="cursor: pointer;">
        <img src="/img/logo.jpeg" alt="AgriCulture" class="">
      </a>

      <nav id="navmenu" class="navmenu">
        <ul>
          <li><router-link :to="{name: 'home'}">Home</router-link></li>
          <li><router-link :to="{name: 'about'}">About Us</router-link></li>
          <li><router-link :to="{name: 'services'}" class="">Our Services</router-link></li>

<!--          <li class="dropdown"><a href="#"><span>Dropdown</span> <i class="bi bi-chevron-down toggle-dropdown"></i></a>-->
<!--            <ul>-->
<!--              <li><a href="#">Dropdown 1</a></li>-->
<!--              <li class="dropdown"><a href="#"><span>Deep Dropdown</span> <i class="bi bi-chevron-down toggle-dropdown"></i></a>-->
<!--                <ul>-->
<!--                  <li><a href="#">Deep Dropdown 1</a></li>-->
<!--                  <li><a href="#">Deep Dropdown 2</a></li>-->
<!--                  <li><a href="#">Deep Dropdown 3</a></li>-->
<!--                  <li><a href="#">Deep Dropdown 4</a></li>-->
<!--                  <li><a href="#">Deep Dropdown 5</a></li>-->
<!--                </ul>-->
<!--              </li>-->
<!--              <li><a href="#">Dropdown 2</a></li>-->
<!--              <li><a href="#">Dropdown 3</a></li>-->
<!--              <li><a href="#">Dropdown 4</a></li>-->
<!--            </ul>-->
<!--          </li>-->
          <li><router-link :to="{name: 'contact'}">Contact</router-link></li>
        </ul>
        <i class="mobile-nav-toggle d-xl-none bi bi-list"></i>
      </nav>

    </div>
  </header>
</template>
