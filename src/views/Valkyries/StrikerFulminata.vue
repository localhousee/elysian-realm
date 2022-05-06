<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script>
import Card from "../../components/Card.vue";

const valkyrie = {
  name: "Striker Fulminata",
  imageSrc: "/images/striker-fulminata.jpeg",
  imageAlt: "Striker Fulminata",
  position: "object-center",
};
</script>