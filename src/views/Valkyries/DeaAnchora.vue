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
			id: 3,
			name: 'Dea Anchora',
			imageSrc: './public/images/dea-anchora.jpg',
			imageAlt: 'Dea Anchora',
			position: 'object-right-top',
		};

		return {
			valkyrie,
		};
	}
}
</script>