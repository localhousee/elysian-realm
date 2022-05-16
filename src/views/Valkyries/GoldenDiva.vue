<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "193a77a8-020d-4f1f-b47c-f602694efee6",
  name: "Golden Diva",
  imageSrc: "/images/golden-diva.jpg",
  imageAlt: "Golden Diva",
  position: "object-center",
};

const signets = {};
</script>