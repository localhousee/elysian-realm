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
			id: 10,
			name: 'Luna Kindred',
			imageSrc: './public/images/luna-kindred.png',
			imageAlt: 'Luna Kindred',
			position: 'object-[-11rem]',
		};

		return {
			valkyrie,
		};
	}
}
</script>