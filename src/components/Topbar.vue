<template>
  <header>
    <div class="header container">
      <div class="logo">
        <h2>Flair</h2>
      </div>

      <div class="controls">
        <div class="nav-links">
          <a href="#" @click="lenis.scrollTo('#work')" class="nav-link">
            Talent</a
          >
          <a href="#" @click="lenis.scrollTo('#skills')" class="nav-link">
            Models</a
          >
          <a href="#" @click="lenis.scrollTo('#contact')" class="nav-link">
            News</a
          >
          <a href="#" @click="lenis.scrollTo('#contact')" class="nav-link">
            Partners</a
          >
        </div>

        <div class="header-buttons">
          <a target="_blank" href="/AnuoluwapoAbolarin.pdf">
            <button type="button" class="btn btn_contact">
              <span>Contact Us</span>
            </button>
          </a>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
// import { onMounted } from "vue";
// import { lenis } from "../helpers/animations";
</script>

<style></style>
