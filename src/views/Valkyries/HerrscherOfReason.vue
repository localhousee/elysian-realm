<template>
<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
	import Card from '../../components/Card.vue';

	const valkyrie = {
		id: 6,
		name: 'Herrscher Of Reason',
		imageSrc: './src/assets/images/herrscher-of-reason.jpg',
		imageAlt: 'Herrscher Of Reason',
		position: 'object-center',
	};

	const signets = {
		builds: [
			{
				id: 1,
				name: 'Evade',
				signets: [
					{
						id: 1,
						name: 'Kevin 1',
						lists: [
							{
								id: 1,
								name: 'Artifact of the Inhibitor',
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
			},
			{
				id: 2,
				name: 'Ultimate',
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
			},
		]
	};
</script>