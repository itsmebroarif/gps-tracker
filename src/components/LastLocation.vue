<template>
  <div id="map" style="height: 500px"></div>
</template>

<script setup>
import { onMounted } from "vue";
import L from "leaflet";

onMounted(() => {
  const map = L.map("map").setView([-6.402, 106.794], 13); // Ganti koordinat sesuai kebutuhan

  L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
    attribution: "© OpenStreetMap contributors",
  }).addTo(map);

  // Gunakan icon mobil bawaan Leaflet (atau custom jika ingin)
  const carIcon = L.divIcon({
    html: '<div style="font-size: 40px;">🚗</div>',
    className: "",
    iconSize: [25, 25],
  });

  // Tambahkan marker mobil
  L.marker([-6.402, 106.794], { icon: carIcon })
    .addTo(map)
    .bindPopup("<b>Mobil Terakhir Terlihat</b><br>Depok")
    .openPopup();
});
</script>
