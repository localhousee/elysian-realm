<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "841657d8-9dbf-4d77-ae23-3efed86503da",
  name: "Silverwing: N-EX",
  imageSrc: "/images/silverwing-nex.jpg",
  imageAlt: "Silverwing: N-EX",
  position: "object-center",
};

const signets = {};
</script>