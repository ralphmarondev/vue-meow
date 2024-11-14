<script setup lang="ts">
import {ref} from "vue"
import VueCal from "vue-cal";

const selectedDate = ref(null)
const events = ref([
  {start: '2024-11-14T10:00:00', end: '2024-11-14T10:00:00', title: 'Sample Event'},
  {start: '2024-11-15T10:00:00', end: '2024-11-15T10:00:00', title: 'Sample Event'}
])

// const disabledDates = ref([
//   '2024-11-16',
//   '2024-11-17'
// ])
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
          <div class="btn-group text-center">
            <button class="btn btn-outline-primary btn-sm dropdown-toggle" type="button" id="dropdownMenuCalendar"
                    data-bs-toggle="dropdown" aria-expanded="false">Thu 11:03
            </button>
            <div class="dropdown-menu">
              <VueCal
                  v-model="selectedDate"
                  :events="events"
                  :show-today="true"
                  mode="month"
                  :show-week-number="false"
                  :show-day-names="true"
                  :disable-month-change="true"
                  :disable-year-change="true"
                  :show-header="false"
              />
            </div>
          </div>
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