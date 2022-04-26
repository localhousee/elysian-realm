<template>
<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
	import Card from '../../components/Card.vue';

	const valkyrie = {
		id: 1,
		name: 'Argent Knight: Artemis',
		imageSrc: './src/assets/images/argent-knight-artemis.jpg',
		imageAlt: 'Argent Knight: Artemis',
		position: 'object-center',
	};
	
	const signets = {
		builds: [
			{
				id: 1,
				name: 'Recommendation',
				signets: [
					{
						id: 1,
						name: 'Su 2',
						lists: [
							{
								id: 1,
								name: 'Motto of Dibba-Cakkhu',
								priority: 'YES',
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
	};
</script>