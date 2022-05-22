<template>
  <TabGroup>
    <TabList
      class="flex p-1 space-x-1 bg-slate-800 rounded-xl"
    >
      <Tab
        v-for="(signet, index) in signets.builds"
        as="template"
        :key="index"
        v-slot="{ selected }"
      >
        <button
          :class="[
            'w-full py-2.5 text-sm leading-5 font-semibold uppercase rounded-lg',
            'focus:outline-none',
            selected ? 'bg-slate-600 text-white' : 'text-white',
          ]"
        >
          {{ signet.name }}
        </button>
      </Tab>
    </TabList>

    <TabPanels class="mt-2">
      <TabPanel
        v-for="(signet, index) in signets.builds"
        :key="index"
        :class="[
          'dark:bg-slate-800 rounded-xl p-3',
          'focus:outline-none',
        ]"
      >
        <div class="relative p-3 rounded-md">
          <Support :support="signet.supports" />
        </div>
        <div
          v-for="(sign, index) in signet.signets"
          :key="index"
          class="relative p-3 rounded-md"
        >
          <Signet :signet="sign" />
        </div>
      </TabPanel>
    </TabPanels>
  </TabGroup>
</template>
<script setup>
import { ref } from "vue";
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from "@headlessui/vue";
import Support from "./Support.vue";
import Signet from "./Signet.vue";

defineProps({
  signets: Object,
});
</script>