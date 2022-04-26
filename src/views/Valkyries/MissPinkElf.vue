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
			id: 12,
			name: 'Miss Pink Elf',
			imageSrc: './public/images/miss-pink-elf.jpg',
			imageAlt: 'Miss Pink Elf',
			position: 'object-center',
		};

		return {
			valkyrie,
		};
	}
}
</script>