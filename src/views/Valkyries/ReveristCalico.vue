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
			id: 15,
			name: 'Reverist Calico',
			imageSrc: '/images/reverist-calico.jpg',
			imageAlt: 'Reverist Calico',
			position: 'object-[-8rem]',
		};

		return {
			valkyrie,
		};
	}
}
</script>