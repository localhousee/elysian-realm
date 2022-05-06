<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script>
import Card from "../../components/Card.vue";

const valkyrie = {
  name: "Spina Astera",
  imageSrc: "/images/spina-astera.jpg",
  imageAlt: "Spina Astera",
  position: "object-top",
};
</script>