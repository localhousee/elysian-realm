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
			id: 4,
			name: 'Fallen Rosemary',
			imageSrc: './public/images/fallen-rosemary.png',
			imageAlt: 'Fallen Rosemary',
			position: 'object-center',
		};

		return {
			valkyrie,
		};
	}
}
</script>