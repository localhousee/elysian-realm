<template>
  <Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script>
import Card from "../../components/Card.vue";

const valkyrie = {
  name: "Prinzessin der Verurteilung",
  imageSrc: "/images/prinzessin-der-verurteilung.jpg",
  imageAlt: "Prinzessin der Verurteilung",
  position: "object-right-top",
};
</script>