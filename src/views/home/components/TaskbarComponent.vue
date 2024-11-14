<script setup lang="ts">

</script>

<template>
  <div class="taskbar mt-3">
    <div class="col">
      <div class="row">
        <div class="mb-3">
          <button class="btn btn-secondary btn-block">
            <img src="@/assets/images/cat.png" alt="Cat" class="sample-app-icon">
          </button>
        </div>
        <div class="mb-3">
          <button class="btn btn-secondary btn-block">
            <img src="@/assets/images/folder.png" alt="Folder" class="sample-app-icon">
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.taskbar {
  position: absolute;
  z-index: 3;
}

.sample-app-icon {
  width: 48px;
  height: 48px;
  border-radius: 5px;
  background: transparent;
  object-fit: cover;
}

</style>