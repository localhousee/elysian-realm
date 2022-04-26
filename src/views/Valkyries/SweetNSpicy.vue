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
			id: 22,
			name: 'Sweet N Spicy',
			imageSrc: './public/images/sweet-n-spicy.jpg',
			imageAlt: 'Sweet N Spicy',
			position: 'object-[-3rem]',
		};

		return {
			valkyrie,
		};
	}
}
</script>