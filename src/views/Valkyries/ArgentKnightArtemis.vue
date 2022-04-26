<template>
<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
	import Card from '../../components/Card.vue';

	const valkyrie = {
		id: 1,
		name: 'Argent Knight: Artemis',
		imageSrc: '/images/argent-knight-artemis.jpg',
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
						name: 'Elysia',
						lists: [
							{
								id: 1,
								name: 'Blessing of Winter Harvest',
								priority: 'Start',
							},
							{
								id: 2,
								name: 'Blessing of Stellar Trials',
								priority: '1st'
							},
							{
								id: 3,
								name: 'Blessing of Frost Scythe',
								priority: '2nd'
							},
							{
								id: 4,
								name: 'Blessing of Uranian Mirror',
								priority: 'Filler'
							},
							{
								id: 5,
								name: 'Blessing of Cold Moon',
								priority: 'Optional'
							}
						],
					},
					{
						id: 2,
						name: 'Mobius 1',
						lists: [
							{
								id: 1,
								name: 'Lip Poison [E]',
								priority: '1st',
							},
							{
								id: 2,
								name: 'Lodging [C]',
								priority: '2nd'
							},
							{
								id: 3,
								name: 'Entwined [P]',
								priority: '3rd'
							},
							{
								id: 4,
								name: 'Infinite [X]',
								priority: null
							},
							{
								id: 5,
								name: 'Dead [X]',
								priority: 'YES'
							},
							{
								id: 6,
								name: 'Newborn [X]',
								priority: 'Filler'
							}
						],
					},
					{
						id: 3,
						name: 'Kevin 2',
						lists: [
							{
								id: 1,
								name: 'Rochet of the Pilgrim',
								priority: 'YES'
							},
							{
								id: 2,
								name: 'Artifact of the Inhibitor',
								priority: '1st'
							},
							{
								id: 3,
								name: 'Brand of the Undead',
								priority: '2nd'
							},
							{
								id: 4,
								name: 'Goblet of the Giver',
								priority: '3rd'
							},
							{
								id: 5,
								name: 'Shadow of the Deliverer',
								priority: null
							},
							{
								id: 6,
								name: 'Dream of the Deliverer',
								priority: 'YES'
							},
						],
					},
					{
						id: 4,
						name: 'Eden 2',
						lists: [
							{
								id: 1,
								name: 'Recitatif of Creeks',
								priority: '1st'
							},
							{
								id: 2,
								name: 'Recitatif of Eden',
								priority: '2nd'
							},
							{
								id: 3,
								name: 'Recitatif of Fine Jade',
								priority: '3rd'
							},
							{
								id: 4,
								name: 'Echo of Gold',
								priority: null
							},
							{
								id: 5,
								name: 'Echo of Silent Night',
								priority: '1st'
							},
							{
								id: 6,
								name: 'Echo of Withered Soil',
								priority: 'Filler'
							},
						],
					},
					{
						id: 5,
						name: 'Su 2',
						lists: [
							{
								id: 1,
								name: 'Motto of Dibba-Cakkhu',
								priority: '1st'
							},
							{
								id: 2,
								name: 'Motto of Asavakkhaya',
								priority: '2nd'
							},
							{
								id: 3,
								name: 'Motto of Iddhi-Vidha',
								priority: '3rd'
							},
							{
								id: 4,
								name: 'Dictum of Bodhi',
								priority: null
							},
							{
								id: 5,
								name: 'Dictum of Anatman',
								priority: 'Optional'
							},
						],
					}
				]
			}
		]
	};
</script>