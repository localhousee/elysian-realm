<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from "../../components/Card.vue";

const valkyrie = {
  id: "3d4d0ed7-e673-4d74-90fd-8143ce884e55",
  name: "Disciplinary Perdition",
  imageSrc: "/images/disciplinary-perdition.jpg",
  imageAlt: "Disciplinary Perdition",
  position: "object-top",
};

const signets = {};
</script>