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
			id: 9,
			name: 'Infinite Ouroboros',
			imageSrc: '/images/infinite-ouroboros.png',
			imageAlt: 'Infinite Ouroboros',
			position: 'object-[-10rem]',
		};

		return {
			valkyrie,
		};
	}
}
</script>