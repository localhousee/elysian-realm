<template>
<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
import Card from '../../components/Card.vue';

const valkyrie = {
	id: 23,
	name: 'Twilight Paladin',
	imageSrc: '/images/twilight-paladin.png',
	imageAlt: 'Twilight Paladin',
	position: 'object-right',
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
							name: 'Blessing of Penalty',
							desc: 'In Fervent state, Total DMG increases by 15% per second for up to 10 stacks. Reset when exiting Fervent state',
							priority: 'Start'
						},
						{
							id: 2,
							name: 'Blessing of Dusk',
							desc: 'With Polarization Agent consumed, Feverish Barrage deals ATK of bonus Physical DMG and grants 10% bonus Move Speed for 20s. 6 stacks max',
							priority: '1st'
						},
						{
							id: 3,
							name: 'Blessing of Banishment',
							desc: 'Every combo hits reduce Ultimate CD by 18% and restore 5 SP. CD: 2s. Ultimate deal 100% bonus Physical DMG and an additional 3000% ATK of Physical DMG. Blood Tide continuously gathers enemies nearby',
							priority: '2nd'
						},
						{
							id: 4,
							name: 'Blessing of Radiance',
							desc: 'Ultimate Evasion Skill resets Fervor drain speed, boosts Physical DMG by 80% for 8s. Casting Feverish Barrage in Fervent state triggers Ultimate Evasion Skill but not Fang Execution',
							priority: 'No'
						},
						{
							id: 5,
							name: 'Blessing of Sanction',
							desc: 'Every combo hits trigger slashing blades to deal 2x1000% ATK of Physical DMG and grant 30% Physical Breach lasting 1s. CD: 5s',
							priority: 'No'
						},
					],
				},
				{
					id: 2,
					name: 'Su 2',
					lists: [
						{
							id: 1,
							name: 'Motto of Dibba-Cakkhu',
							desc: 'Combo hits are reset at to boost Total DMG taken by all enemies by 35% for 10s',
							priority: '1st'
						},
						{
							id: 2,
							name: 'Motto of Asavakkhaya',
							desc: 'Attacks grant 25 bonus combo hits on hit. CD: 5s',
							priority: '2nd'
						},
						{
							id: 3,
							name: 'Motto of Iddhi-Vidha',
							desc: 'Combo hits are increased to 60 when below 60. CD: 10s',
							priority: '3rd'
						},
						{
							id: 4,
							name: 'Dictum of Bodhi',
							desc: '',
							priority: ''
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
							desc: 'Using a weapon active taints enemies nearby with red paint for 8s and makes them take 25% bonus Physical and Elemental MG (cannot stack). Triggering it again resets the duration',
							priority: '1st'
						},
						{
							id: 2,
							name: 'Yellow & Warm',
							desc: 'Using an Ultimate taints enemies nearby with yellow paint for 8s and makes them take 30% bonus Total DMG. Triggering it again resets the duration',
							priority: '2nd'
						},
						{
							id: 3,
							name: 'Grey & Empty',
							desc: 'Enemies stay tainted for 5s longer',
							priority: '3rd'
						},
						{
							id: 4,
							name: 'Blue & Cold',
							desc: 'Triggering an Ultimate Evasion Skill taints enemies nearby with blue paint for 8s and reduces their Total DMG and Move Speed by 30%. Triggering it again resets the duration',
							priority: '4th'
						},
						{
							id: 5,
							name: 'Shine like Stars',
							desc: 'Entering Sprint triggers Stage 2 and until Sprint ends, attacks cost 40 Resolve more on hit to deal 2000% ATK of Fire DMG per second',
							priority: ''
						},
						{
							id: 6,
							name: 'Blooming like Flowers',
							desc: 'When enemies of countering types are tainted with both blue and red paints, Valkyries deal 50% bonus Total DMG to them (cannot stack)',
							priority: 'Yes'
						}
					],
				},
				{
					id: 4,
					name: 'Eden 2',
					lists: [
						{
							id: 1,
							name: 'Recitatif of Creeks',
							desc: 'Every 10 SP left boosts Physical & Elemental DMG by 2.5%',
							priority: '1st'
						},
						{
							id: 2,
							name: 'Recitatif of Eden',
							desc: 'Every 10 SP left boosts Total DMG by 3.0%',
							priority: '2nd'
						},
						{
							id: 3,
							name: 'Recitatif of Fine Jade',
							desc: 'Initial SP and max SP increase by 30',
							priority: '3rd'
						},
						{
							id: 4,
							name: 'Echo of Gold',
							desc: '',
							priority: ''
						},
						{
							id: 5,
							name: 'Echo of Silent Night',
							desc: 'After lasting over 7s, reduce ATK, DEF, ele resists of enemies nearby',
							priority: '1st'
						},
						{
							id: 6,
							name: 'Echo of Gold',
							desc: 'After lasting over 7s, boost SP cap and restore SP/s till it ends',
							priority: 'Filler'
						},
					],
				},
				{
					id: 5,
					name: 'Kevin 1',
					lists: [
						{
							id: 1,
							name: 'Artifact of the Inhibitor',
							desc: 'Ultimate boosts Elemental Breach by 25% for 5s',
							priority: '1st'
						},
						{
							id: 2,
							name: 'Brand of the Undead',
							desc: 'Ultimate boosts Elemental DMG by 30% for 5s',
							priority: '2nd'
						},
						{
							id: 3,
							name: 'Goblet of the Giver',
							desc: 'Ultimate boosts Total DMG by 35% for 5s',
							priority: '3rd'
						},
						{
							id: 4,
							name: 'Blade of the Deliverer',
							desc: '',
							priority: '4th'
						},
						{
							id: 5,
							name: 'Echo of the Deliverer',
							desc: 'Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s',
							priority: '1st'
						},
						{
							id: 6,
							name: 'Crusade of the Deliverer',
							desc: 'After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%',
							priority: '2nd'
						},
					],
				},
			]
		}
	]
}
</script>