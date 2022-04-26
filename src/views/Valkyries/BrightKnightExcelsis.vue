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
			id: 2,
			name: 'Bright Knight: Excelsis',
			imageSrc: './src/assets/images/bright-knight-excelsis.jpg',
			imageAlt: 'Bright Knight: Excelsis',
			position: 'object-center',
		};

		return {
			valkyrie,
		};
	}
}
</script>