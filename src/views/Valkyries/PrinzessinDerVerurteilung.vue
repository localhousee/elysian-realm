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
			id: 14,
			name: 'Prinzessin der Verurteilung',
			imageSrc: '/images/prinzessin-der-verurteilung.jpg',
			imageAlt: 'Prinzessin der Verurteilung',
			position: 'object-top',
		};

		return {
			valkyrie,
		};
	}
}
</script>