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
			id: 17,
			name: 'Silverwing: N-EX',
			imageSrc: './src/assets/images/silverwing-nex.jpg',
			imageAlt: 'Silverwing: N-EX',
			position: 'object-center',
		};

		return {
			valkyrie,
		};
	}
}
</script>