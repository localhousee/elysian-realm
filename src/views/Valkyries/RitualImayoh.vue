<template>
<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script>
import Card from '../../components/Card.vue';

export default {
	components: {
		Card,
	},

	setup() {
		const valkyrie = {
			id: 16,
			name: 'Ritual Imayoh',
			imageSrc: '/images/ritual-imayoh.jpg',
			imageAlt: 'Ritual Imayoh',
			position: 'object-right-top',
		};

		return {
			valkyrie,
		};
	}
}
</script>