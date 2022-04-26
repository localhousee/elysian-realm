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
			id: 7,
			name: 'Herrscher Of Sentience',
			imageSrc: './public/images/herrscher-of-sentience.jpg',
			imageAlt: 'Herrscher Of Sentience',
			position: 'object-top',
		};

		return {
			valkyrie,
		};
	}
}
</script>