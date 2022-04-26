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
			id: 19,
			name: 'Starchasm Nyx',
			imageSrc: '/images/starchasm-nyx.png',
			imageAlt: 'Starchasm Nyx',
			position: 'object-[-4rem]',
		};

		return {
			valkyrie,
		};
	}
}
</script>