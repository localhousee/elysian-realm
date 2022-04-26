<template>
 <TabGroup>
	<TabList class="flex p-1 space-x-1 bg-blue-700 rounded-xl">
		<Tab
			v-for="signet in signets.builds"
			as="template"
			:key="signet.id"
			v-slot="{ selected }"
		>
			<button
				:class="[
					'w-full py-2.5 text-sm leading-5 font-medium text-blue-700 rounded-lg',
					'focus:outline-none focus:ring-2 ring-offset-2 ring-offset-blue-400 ring-white ring-opacity-60',
					selected
						? 'bg-white shadow'
						: 'text-blue-100 hover:bg-white/[0.12] hover:text-white',
				]"
			>
				{{ signet.name }}
			</button>
		</Tab>
	</TabList>

	<TabPanels class="mt-2">
		<div v-for="signet in signet.signets" :key="signet.id">

		<TabPanel
			:class="[
				'bg-white rounded-xl p-3',
				'focus:outline-none focus:ring-2 ring-offset-2 ring-offset-blue-400 ring-white ring-opacity-60',
			]"
		>
			<p class="font-bold text-center text-sm text-blue-900 pb-4 uppercase" v-text="signet.name" />
			<Signet :signet="signet" />
		</TabPanel>
		</div>
	</TabPanels>
</TabGroup>	
</template>

<script setup>
import { TabGroup, TabList, TabPanel, Tab } from '@headlessui/vue'
import Signet from './Signet.vue'

defineProps({
	signets: Array,
})
</script>

