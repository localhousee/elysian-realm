<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "d218fff3-9947-40d9-9f6e-7eb14badfe33",
  name: "Griseo",
  imageSrc: "/images/griseo.jpg",
  imageAlt: "Griseo",
  position: "object-center",
};

const signets = {};
</script>
