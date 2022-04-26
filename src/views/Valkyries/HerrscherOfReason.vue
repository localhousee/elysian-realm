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
						name: 'Elysia',
						lists: [
							{
								id: 1,
								name: 'Blessing of Truth',
								priority: 'Start',
							},
							{
								id: 2,
								name: 'Blessing of Inspiration',
								priority: '1st'
							},
							{
								id: 3,
								name: 'Blessing of Reason',
								priority: '2nd'
							},
							{
								id: 4,
								name: 'Blessing of Creation',
								priority: 'Filler'
							},
							{
								id: 5,
								name: 'Blessing of Wisdom',
								priority: 'No'
							}
						],
					},
					{
						id: 2,
						name: 'Sakura 2',
						lists: [
							{
								id: 1,
								name: 'Bountiful Blossom: Fuji',
								priority: '1st',
							},
							{
								id: 2,
								name: 'Bountiful Blossom: Ayame',
								priority: '1st',
							},
							{
								id: 3,
								name: 'Bountiful Blossom: Kiku',
								priority: '2nd'
							},
							{
								id: 4,
								name: 'Bountiful Blossom: Koyo',
								priority: '3rd'
							},
							{
								id: 5,
								name: 'Setsuna blade: Yasha',
								priority: null
							},
						],
					},
					{
						id: 3,
						name: 'Griseo 1',
						lists: [
							{
								id: 1,
								name: 'Red & Hot',
								priority: '1st'
							},
							{
								id: 2,
								name: 'Yellow & Warm',
								priority: '2nd'
							},
							{
								id: 3,
								name: 'Grey & Empty',
								priority: '3rd'
							},
							{
								id: 4,
								name: 'Blue & Cold',
								priority: '4th'
							},
							{
								id: 5,
								name: 'Shine like Stars',
								priority: null
							},
							{
								id: 6,
								name: 'Blooming like Flowers',
								priority: 'YES'
							},
						],
					},
					{
						id: 4,
						name: 'Hua 2',
						lists: [
							{
								id: 1,
								name: 'Old Dreams Again',
								priority: '1st'
							},
							{
								id: 2,
								name: 'Lost and Found',
								priority: '2nd'
							},
							{
								id: 3,
								name: 'Suffering Mass',
								priority: null
							},
							{
								id: 4,
								name: 'Worldly Troubles',
								priority: '1st'
							},
							{
								id: 5,
								name: 'Broken Dream',
								priority: '2nd'
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
						name: 'Elysia',
						lists: [
							{
								id: 1,
								name: 'Blessing of Truth',
								priority: 'Start',
							},
							{
								id: 2,
								name: 'Blessing of Inspiration',
								priority: '1st'
							},
							{
								id: 3,
								name: 'Blessing of Wisdom',
								priority: '2nd'
							},
							{
								id: 4,
								name: 'Blessing of Reason',
								priority: '3rd'
							},
							{
								id: 5,
								name: 'Blessing of Creation',
								priority: 'No'
							}
						],
					},
					{
						id: 2,
						name: 'Griseo 1',
						lists: [
							{
								id: 1,
								name: 'Red & Hot',
								priority: '1st'
							},
							{
								id: 2,
								name: 'Yellow & Warm',
								priority: '2nd'
							},
							{
								id: 3,
								name: 'Grey & Empty',
								priority: '3rd'
							},
							{
								id: 4,
								name: 'Blue & Cold',
								priority: '4th'
							},
							{
								id: 5,
								name: 'Shine like Stars',
								priority: null
							},
							{
								id: 6,
								name: 'Blooming like Flowers',
								priority: 'YES'
							},
						],
					},
					{
						id: 3,
						name: 'Kevin 2',
						lists: [
							{
								id: 1,
								name: 'Artifact of the Inhibitor',
								priority: '1st'
							},
							{
								id: 2,
								name: 'Brand of the Undead',
								priority: '2nd'
							},
							{
								id: 3,
								name: 'Goblet of the Giver',
								priority: '3rd'
							},
							{
								id: 4,
								name: 'Shadow of the Deliverer',
								priority: null
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
						id: 4,
						name: 'Sakura 1',
						lists: [
							{
								id: 1,
								name: 'Bountiful Blossom: Koyo',
								priority: '1st'
							},
							{
								id: 2,
								name: 'Bountiful Blossom: Ayame',
								priority: '2nd'
							},
							{
								id: 3,
								name: 'Bountiful Blossom: Fuji',
								priority: '3rd'
							},
							{
								id: 4,
								name: 'Setsuna Blade: Sakura ni Maku',
								priority: null
							},
							{
								id: 5,
								name: 'Setsuna Blade: Ame-Shiko',
								priority: 'YES'
							},
						],
					},
				]
			},
		]
	};
</script>