<script setup lang="ts">
import HeaderComponent from "@/views/home/components/HeaderComponent.vue"
import TaskbarComponent from "@/views/home/components/TaskbarComponent.vue"
</script>

<template>
  <div>
    <img src="@/assets/images/wallpaper.png" alt="Wallpaper"
         style="position: absolute; top: 0;left: 0; width: 100vw; height: 100vh; object-fit: cover; z-index: 1"/>
    <HeaderComponent/>
    <div class="container">
      <div class="row">
        <div class="col">
          <TaskbarComponent/>
        </div>
      </div>
    </div>
  </div>
</template>