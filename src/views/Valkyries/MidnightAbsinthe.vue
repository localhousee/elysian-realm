<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script>
import Card from "../../components/Card.vue";

const valkyrie = {
  name: "Midnight Absinthe",
  imageSrc: "/images/midnight-absinthe.jpg",
  imageAlt: "Midnight Absinthe",
  position: "object-[-11rem]",
};
</script>