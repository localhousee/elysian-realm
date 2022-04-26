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
			id: 20,
			name: 'Striker Fulminata',
			imageSrc: './src/assets/images/striker-fulminata.jpeg',
			imageAlt: 'Striker Fulminata',
			position: 'object-center',
		};

		return {
			valkyrie,
		};
	}
}
</script>