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
			id: 11,
			name: 'Midnight Absinthe',
			imageSrc: './src/assets/images/midnight-absinthe.png',
			imageAlt: 'Midnight Absinthe',
			position: 'object-[-11rem]',
		};

		return {
			valkyrie,
		};
	}
}
</script>