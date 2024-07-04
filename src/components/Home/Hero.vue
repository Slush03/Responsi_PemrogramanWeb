<script setup>

import ProfilePic from "@/components/Home/ProfilePic.vue";
</script>

<template>
  <header class="py-5">
    <div class="container px-5 pb-5">
      <div class="row gx-5 align-items-center">
        <div class="col-xxl-5">
          <!-- Header text content-->
          <div class="text-center text-xxl-start">
            <div class="text-white mb-2" style="font-size: 25px; font-weight: bold"><div class="text-uppercase">22.11.IF03 </div></div>
            <div class="fs-3 fw-light text-black">Hello There!👋</div>
            <h1 class="display-6 fw-bolder mb-2">I'm <span class="text-gradient d-inline">Taufiq Kurniawan Akbar</span></h1>
            <div class="fs-3 fw-light text-black mb-2">I'm just a normal Indonesian citizen!</div>
            <div class="d-grid gap-3 d-sm-flex justify-content-sm-center justify-content-xxl-start mb-3">
              <RouterLink to="/resume" class="btn btn-primary btn-lg px-5 py-3 me-sm-3 fs-6 fw-bolder">Resume</RouterLink>
              <RouterLink to="/about" class="btn btn-outline-dark btn-lg px-5 py-3 fs-6 fw-bolder">About Me</RouterLink>
            </div>
          </div>
        </div>
        <div class="col-xxl-7">
          <!-- Header profile picture-->
          <div class="d-flex justify-content-center mt-5 mt-xxl-0">
            <ProfilePic/>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>
