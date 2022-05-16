<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "f485ba64-cf4d-4729-8c72-834b173e27b0",
  name: "Fervent Tempo",
  imageSrc: "/images/fervent-tempo.png",
  imageAlt: "Fervent Tempo",
  position: "object-right",
};

const signets = {};
</script>