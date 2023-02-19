<script setup lang="ts">
import Carousel from '../components/Carousel.vue';
import kaguya3 from '../assets/imgs/kaguya3.png';
import codegeassposter from '../assets/imgs/codegeassposter.jpg';
</script>

<template>
  <main>
    <!-- Carousel -->
    <Carousel />

    <div class="d-flex flex-column flex-md-row">
      <!-- Recents Ratings -->
      <article class="m-3 mt-3">
        <div class="list rounded bg-success p-1">

          <!-- List Header -->
          <div class="list-header">
            <h4 class="py-2 px-2 m-0 text-white">Recent reviews</h4>
          </div>

          <!-- List Body -->
          <div class="list-body px-2 py-1">

            <!-- Card -->
            <div class="card mb-3 border-0 shadow-lg" style="max-width: 540px;">
              <div class="row g-0">
                <div class="col-md-4 col-4">
                  <img :src="kaguya3" class="img-fluid object-fit-cover h-100 rounded-start shadow">
                </div>
                <div class="col-md-8 col-8">
                  <div class="card-body">
                    <h5 class="card-title">Kaguya Sama: Love Is War - Season 3</h5>
                    <p class="card-text">This is a wider card with supporting text below as a natural lead-in to
                      additional
                      content. This content is a little bit longer.</p>
                    <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                  </div>
                </div>
              </div>
            </div>

            <!-- Card -->
            <div class="card border-0 shadow-lg" style="max-width: 540px;">
              <div class="row g-0">
                <div class="col-md-4 col-4">
                  <img :src="codegeassposter" class="img-fluid object-fit-cover h-100 rounded-start shadow">
                </div>
                <div class="col-md-8 col-8">
                  <div class="card-body">
                    <h5 class="card-title">Code Geass: Lelouch of the Rebellion</h5>
                    <p class="card-text">anime da franquia Code Geass, de 2006, com 25 episódios, criado pela Sunrise.
                      Dirigida por Gorō Taniguchi e escrita por Ichirō Ōkouchi...</p>
                    <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                  </div>
                </div>
              </div>
            </div>

          </div>
        </div>
      </article>

      <!-- Popular Ratings -->
      <article class="m-3 mt-3">
        <div class="list rounded bg-success p-1">

          <!-- List Header -->
          <div class="list-header">
            <h4 class="py-2 px-2 m-0 text-white">Popular reviews</h4>
          </div>

          <!-- List Body -->
          <div class="list-body px-2 py-1">

            <!-- Card -->
            <div class="card mb-3 border-0" style="max-width: 540px;">
              <div class="row g-0">
                <div class="col-md-4 col-4">
                  <img :src="kaguya3" class="img-fluid object-fit-cover h-100 rounded-start">
                </div>
                <div class="col-md-8 col-8">
                  <div class="card-body">
                    <h5 class="card-title">Kaguya Sama: Love Is War - Season 3</h5>
                    <p class="card-text">This is a wider card with supporting text below as a natural lead-in to
                      additional
                      content. This content is a little bit longer.</p>
                    <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                  </div>
                </div>
              </div>
            </div>

            <!-- Card -->
            <div class="card border-0" style="max-width: 540px;">
              <div class="row g-0">
                <div class="col-md-4 col-4">
                  <img :src="kaguya3" class="img-fluid object-fit-cover h-100">
                </div>
                <div class="col-md-8 col-8">
                  <div class="card-body">
                    <h5 class="card-title">Kaguya Sama: Love Is War - Season 3</h5>
                    <p class="card-text">This is a wider card with supporting text below as a natural lead-in to
                      additional
                      content. This content is a little bit longer.</p>
                    <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
                  </div>
                </div>
              </div>
            </div>

          </div>
        </div>
      </article>
    </div>

  </main></template>
