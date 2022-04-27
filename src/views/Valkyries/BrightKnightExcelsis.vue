<template>
<Card :valkyrie="valkyrie" :signets="signets" />
</template>

<script setup>
    import Card from '../../components/Card.vue';

    const valkyrie = {
        id: 2,
        name: 'Bright Knight: Excelsis',
        imageSrc: '/images/bright-knight-excelsis.jpg',
        imageAlt: 'Bright Knight: Excelsis',
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
                                name: 'Blessing of Gambit',
                                desc: "Triggering Retaliation or Ultimate Evasion boosts Physical DMG by 25% for 8s. If triggered outside Burst mode, Valkyrie gains Iron Body for 8s; if triggered in Burst mode, Valkyrie additionally unleashes a counterattack cross strike before Phantom Cleave to deal 1200% ATK of Physical DMG",
                                priority: 'Start',
                            },
                            {
                                id: 2,
                                name: 'Blessing of Glory',
                                desc: "In Burst mode, Weapon Active has 70% shorter CD and can deal 2400% ATK of bonus Physical DMG at the cost of 12 SP. Weapon Active gains 4% Total DMG boost per second, and the boost resets when Burst mode is activated again",
                                priority: '1st',
                            },
                            {
                                id: 3,
                                name: 'Blessing of Paragon',
                                desc: "Ultimate grants 5 stacks of Paragon, each of which boosts Total DMG by 4% for 15s",
                                priority: '2nd',
                            },
                            {
                                id: 4,
                                name: 'Blessing of Holy Lance',
                                desc: "During Basic ATK SEQ 4, tap [ATK] repeatedly to thrust the lance at enemies in an increasingly violent manner to deal a total of 6000% ATK of Physical DMG, and Valkyrie is immune to frontal and flank attacks. When Valkyrie's SEQ 4 attack reaches its peak, Basic ATK SEQ 5 will be enhanced to deal 3500% ATK of bonus Physical DMG to enemies in a large area",
                                priority: 'No',
                            },
                            {
                                id: 5,
                                name: 'Blessing of Formation',
                                desc: "Basic ATK SEQ 5 creates a 3-sec Grav Singularity that pulls in surrounding enemies and deals 2100% ATK of Physical DMG to them. Basic ATK SEQ 4 & 5 and the explosion of the Grav Singularity boost Valkyrie's Total DMG by 3% for 40s (15 stacks max)",
                                priority: 'No',
                            }
                        ],
                    },
                    {
                        id: 2,
                        name: 'Kevin 1',
                        lists: [
                            {
                                id: 1,
                                name: 'Mask of the Predator',
                                desc: 'Ultimate boosts Physical Breach by 25% for 5s',
                                priority: '1st',
                            },
                            {
                                id: 2,
                                name: 'Pendant of the Watcher',
                                desc: 'Ultimate boosts Physical DMG by 30% for 5s',
                                priority: '2nd',
                            },
                            {
                                id: 3,
                                name: 'Goblet of the Giver',
                                desc: 'Ultimate boosts Total DMG by 35% for 5s',
                                priority: '3rd',
                            },
                            {
                                id: 4,
                                name: 'Nexus Signet: Blade of the Deliverer',
                                desc: 'Core',
                                priority: '',
                            },
                            {
                                id: 5,
                                name: 'Echo of the Deliverer',
                                desc: 'Duration of Final Battle and all buffs provided by Normal Signets of Deliverance are extended to 8s',
                                priority: 'YES',
                            },
                            {
                                id: 6,
                                name: 'Crusade of the Deliverer',
                                desc: 'After 3s into Final Battle, all buffs provided by Normal Signets of Deliverance increase by 90% instead of 50%',
                                priority: '1st',
                            }
                        ],
                    },
                    {
                        id: 3,
                        name: 'Sakura 1',
                        lists: [
                            {
                                id: 1,
                                name: 'Bountiful Blossom: Koyo', 
                                desc: 'Triggering Ultimate Evasion Skill boosts Total DMG taken by all enemies by 30% for 8s',
                                priority: '1st',
                            },
                            {
                                id: 2,
                                name: 'Bountiful Blossom: Ayame',
                                desc: 'Triggering Ultimate Evasion Skill restores 12.0 bonus SP',
                                priority: '2nd',
                            },
                            {
                                id: 3,
                                name: 'Bountiful Blossom: Fuji',
                                desc: 'Ultimate Evasion Skill has 1 more charge and 10% reduced CD',
                                priority: '3rd',
                            },
                            {
                                id: 4,
                                name: 'Nexus Signet Setsuna Blade: Sakura ni Maku',
                                desc: 'Core',
                                priority: '',
                            },
                            {
                                id: 5,
                                name: 'Setsuna Blade: Ame-Shiko',
                                desc: 'Activating Sakura Screen resets Ultimate CD and weapon active CD',
                                priority: 'YES',
                            },
                        ],
                    },
                    {
                        id: 4,
                        name: 'Griseo 1',
                        lists: [
                            {
                                id: 1,
                                name: 'Red & Hot',
                                desc: 'Using a weapon active taints enemies nearby with red paint for 8s and makes them take 25% bonus Physical and Elemental MG (cannot stack). Triggering it again resets the duration',
                                priority: '1st',
                            },
                            {
                                id: 2,
                                name: 'Yellow & Warm',
                                desc: 'Using an Ultimate taints enemies nearby with yellow paint for 8s and makes them take 30% bonus Total DMG. Triggering it again resets the duration',
                                priority: '2nd',
                            },
                            {
                                id: 3,
                                name: 'Grey & Empty',
                                desc: 'Enemies stay tainted for 5s longer',
                                priority: '3rd',
                            },
                            {
                                id: 4,
                                name: 'Blue & Cold',
                                desc: 'Triggering an Ultimate Evasion Skill taints enemies nearby with blue paint for 8s and reduces their Total DMG and Move Speed by 30%. Triggering it again resets the duration',
                                priority: '4th',
                            },
                            {
                                id: 5,
                                name: 'Nexus Signet: Shine like Stars',
                                desc: 'Core',
                                priority: '',
                            },
                            {
                                id: 6,
                                name: 'Blooming like Flowers',
                                desc: 'When enemies of countering types are tainted with both blue and red paints, Valkyries deal 50% bonus Total DMG to them (cannot stack)',
                                priority: 'YES',
                            },
                        ],
                    },
                    {
                        id: 5,
                        name: 'Kalpas 2',
                        lists: [
                            {
                                id: 1,
                                name: 'Bone, Blood, and Ribbon',
                                desc: 'Every 100 HP loss boosts Physical & Elemental DMG by 0.8%',
                                priority: '1st',
                            },
                            {
                                id: 2,
                                name: 'Blade, Grave, and Scar',
                                desc: 'Every 100 HP loss boosts Total DMG by 1.0%',
                                priority: '2nd',
                            },
                            {
                                id: 3,
                                name: 'Path, Misfortune, and Written Fate',
                                desc: 'Max HP increases by 25%',
                                priority: '3rd',
                            },
                            {
                                id: 4,
                                name: 'Nexus Signet: Soldiers, Scissors, Spoils, and Slaughter',
                                desc: 'Core',
                                priority: '',
                            },
                            {
                                id: 5,
                                name: 'Death, Life, Oblivion, and Existence',
                                desc: 'If [Bloodboil Garment] exceeds 1500, when taking damage, reduces damage taken by 1% of [Bloodboil Garment]',
                                priority: 'Filler',
                            },
                        ],
                    }
                ]
            }
        ]
    };
</script>
