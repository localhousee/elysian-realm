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
			id: 21,
			name: 'Stygian Nymph',
			imageSrc: './public/images/stygian-nymph.png',
			imageAlt: 'Stygian Nymph',
			position: 'object-center',
		};

		return {
			valkyrie,
		};
	}
}
</script>