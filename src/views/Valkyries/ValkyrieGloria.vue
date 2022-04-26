<template>
<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from '../../components/Card.vue';

const valkyrie = {
	id: 24,
	name: 'Valkyrie Gloria',
	imageSrc: './public/images/valkyrie-gloria.jpg',
	imageAlt: 'Valkyrie Gloria',
	position: 'object-[-10rem]',
};

const signets = {
	builds: [
		{
			id: 1,
			name: 'Recommendation',
			signets: [
				{
					id: 1,
					name: 'Kevin 1',
					lists: [
						{
							id: 1,
							name: 'Breach Damage',
							priority: 'YES'
						},
						{
							id: 2,
							name: 'Elemental Damage',
							priority: 'YES'
						},
					],
				},
				{
					id: 2,
					name: 'Eden 1',
					lists: [
						{
							id: 1,
							name: 'SP/sec',
							priority: 'YES'
						},
						{
							id: 2,
							name: 'Starting SP',
							priority: 'YES'
						},
					],
				}
			]
		}
	]
}
</script>