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
			id: 13,
			name: 'Palatinus Equinox',
			imageSrc: './src/assets/images/palatinus-equinox.jpg',
			imageAlt: 'Palatinus Equinox',
			position: 'object-top',
		};

		return {
			valkyrie,
		};
	}
}
</script>