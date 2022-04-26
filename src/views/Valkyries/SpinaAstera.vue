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
			id: 18,
			name: 'Spina Astera',
			imageSrc: '/images/spina-astera.jpg',
			imageAlt: 'Spina Astera',
			position: 'object-top',
		};

		return {
			valkyrie,
		};
	}
}
</script>