<script setup lang="ts">

</script>

<template>
  <div>
    <div class="container">
      <div class="row py-1">
        <div class="col md-2 px-2">
          <div class="btn-group ms-2">
            <button class="btn btn-outline-primary btn-sm dropdown-toggle" type="button" id="dropdownMenuButton"
                    data-bs-toggle="dropdown"
                    aria-expanded="false">Activities
            </button>
            <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
              <a href="#" class="dropdown-item">Programming</a>
              <a href="#" class="dropdown-item">Social</a>
              <a href="#" class="dropdown-item">Office</a>
              <div class="dropdown-divider"></div>
              <a href="#" class="dropdown-item">Others</a>
            </div>
          </div>
        </div>
        <div class="col md-7 text-center px-2">
          <button class="btn btn-outline-primary btn-sm">Fri 09:54</button>
        </div>
        <div class="col-md-3 text-end px-2">
          <div class="btn-group me-2">
            <button class="btn btn-outline-primary btn-sm dropdown-toggle px-3" type="button" id="dropdownMenuPower"
                    data-bs-toggle="dropdown" aria-expanded="false">
              Power
            </button>
            <div class="dropdown-menu" aria-labelledby="dropdownMenuPower">
              <a href="#" class="dropdown-item">Suspend</a>
              <a href="#" class="dropdown-item">Shutdown</a>
              <a href="#" class="dropdown-item">Restart</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  position: relative;
  z-index: 2;
  background-color: rgba(255, 255, 255, 0.7);
  border-radius: 8px;
}

.btn-group {
  z-index: 4;
}

.btn.dropdown-toggle::after {
  display: none;
}
</style>