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
			id: 5,
			name: 'Herrscher of Flamescion',
			imageSrc: './src/assets/images/herrscher-of-flamescion.jpg',
			imageAlt: 'Herrscher of Flamescion',
			position: 'object-[-4rem]',
		};

		return {
			valkyrie,
		};
	}
}
</script>