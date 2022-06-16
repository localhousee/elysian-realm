<template>
  <Disclosure v-slot="{ open }" as="div" class="group">
    <DisclosureButton class="
        flex
        justify-between
        w-full
        px-4
        py-2
        text-sm
        font-medium
        text-left
        bg-slate-300
        group-hover:bg-slate-600
        group-hover:text-white
        dark:bg-slate-900
        text-slate-900
        dark:text-white
        dark:hover:bg-slate-700
        rounded-lg
        focus:outline-none
        focus-visible:ring
      ">
      <span>Supports</span>
      <ChevronUpIcon :class="open ? 'transform rotate-180' : ''"
        class="w-5 h-5 text-slate-900 group-hover:text-white dark:text-white" />
    </DisclosureButton>
    <DisclosurePanel class="px-4 text-sm flex bg-transparent">
      <div class="flex-col w-full">
        <div
          class="mt-2 text-slate-100 bg-cyan-600 dark:bg-gray-700 dark:text-white rounded-lg mb-2 flex items-center py-2"
          v-if="support.recommended || support.boss">
          <div class="px-2">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-white" fill="none" viewBox="0 0 24 24"
              stroke="currentColor" stroke-width="2">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>
          </div>
          <div class="flex flex-col">
            <span>Flamechaser: {{ support.boss }}</span>
            <span>Recommended: {{ support.recommended }}</span>
          </div>
        </div>
        <table class="table-auto w-full mt-2">
          <thead>
            <tr class="uppercase bg-gray-300 dark:bg-gray-800 dark:text-gray-100">
              <th class="border border-slate-600 py-2">Time</th>
              <th class="border border-slate-600 py-2">Sigils</th>
              <th class="border border-slate-600 py-2" colspan="2">Supports</th>
            </tr>
          </thead>
          <tbody>
            <tr class="text-center dark:text-white" v-for="(supp, index) in support.supports" :key="index">
              <td class="py-1 border border-slate-600 w-12">
                <span v-text="supp.time" />
              </td>
              <td class="py-1 border border-slate-600">
                <span v-text="supp.sigils" />
              </td>
              <td class="py-1 border border-slate-600 w-16 font-semibold">
                <span v-text="supp.support_1" />
              </td>
              <td class="py-1 border border-slate-600 w-16 font-semibold">
                <span v-text="supp.support_2" />
              </td>
  
            </tr>
          </tbody>
        </table>
      </div>
    </DisclosurePanel>
  </Disclosure>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from "@headlessui/vue";
import { ChevronUpIcon } from "@heroicons/vue/solid";

defineProps({
  support: Array,
});
</script>
