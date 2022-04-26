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
			id: 8,
			name: 'Herrscher Of Thunder',
			imageSrc: './public/images/herrscher-of-thunder.jpg',
			imageAlt: 'Herrscher Of Thunder',
			position: 'object-top',
		};

		return {
			valkyrie,
		};
	}
}
</script>