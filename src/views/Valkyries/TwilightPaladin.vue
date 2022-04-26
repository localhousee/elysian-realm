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
			id: 23,
			name: 'Twilight Paladin',
			imageSrc: '/images/twilight-paladin.png',
			imageAlt: 'Twilight Paladin',
			position: 'object-right',
		};

		return {
			valkyrie,
		};
	}
}
</script>