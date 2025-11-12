<template>
  <div class="col-md-3 d-flex">
    <div class="card hover-shadow flex-fill">
      <img :src="project.image" class="card-img-top card-img">
      <div class="card-body">
        <h5 class="card-title">{{ project.title }}</h5>
        <p class="card-text">{{ project.description }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
import { defineProps } from 'vue';

defineProps({
  project: Object
});
</script>

<style>
.hover-shadow:hover {
  transform: translateY(-5px);
  transition: all 0.3s ease;
  box-shadow: 0 10px 20px rgba(0,0,0,0.2);
}
</style>
