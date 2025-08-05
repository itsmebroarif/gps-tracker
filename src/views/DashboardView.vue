<template>
  <div class="container my-4">
    <!-- Header -->
    <div class="row mb-3">
      <div class="col">
        <h3 class="fw-bold">Arif Permana Putrasuryana</h3>
        <p class="text-muted mb-0">0858-1704-8266</p>
      </div>
    </div>

    <!-- Layout 3 kolom -->
    <div class="row">
      <!-- Kiri: Driver Details -->
      <div class="col-lg-3 mb-3">
        <div class="custom-card h-100">
          <div class="card-body">
            <DriverDetails />
          </div>
        </div>
      </div>

      <!-- Tengah: Last Location -->
      <div class="col-lg-6 mb-3">
        <div class="custom-card h-100">
          <div class="card-body">
            <LastLocation />
          </div>
        </div>
      </div>

      <!-- Kanan: Timeline -->
      <div class="col-lg-3 mb-3">
        <div class="custom-card h-100">
          <div class="card-body">
            <DriverActivityTimeline />
          </div>
        </div>
      </div>
    </div>

    <!-- Bawah: Behavior -->
    <div class="row mt-4">
      <div class="col-12 mb-3">
        <div class="custom-card">
          <div class="card-body">
            <DriverBehavior />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import DriverDetails from "@/components/DriverDetails.vue";
import LastLocation from "@/components/LastLocation.vue";
import DriverBehavior from "@/components/DriverBehavior.vue";
import DriverActivityTimeline from "@/components/DriverActivityTimeline.vue";
</script>

<style scoped>
.custom-card {
  border: 2px solid #dee2e6; /* Lebih tebal dari default */
  border-radius: 1rem; /* Rounded lebih smooth */
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.1); /* Medium shadow */
  background-color: #fff;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.custom-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 24px rgba(0, 0, 0, 0.12);
}

.card-body {
  padding: 1.5rem;
}
</style>
