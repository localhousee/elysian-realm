<template>
  <Disclosure v-slot="{ open }" as="div" class="group">
    <DisclosureButton
      class="
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
      "
    >
      <span>{{ signet.name }}</span>
      <ChevronUpIcon
        :class="open ? 'transform rotate-180' : ''"
        class="w-5 h-5 text-slate-900 group-hover:text-white"
      />
    </DisclosureButton>
    <DisclosurePanel class="px-4 text-sm flex flex-col bg-white dark:bg-slate-800">
      <div
        class="mt-2 text-slate-100 bg-cyan-600 dark:bg-gray-700 dark:text-white rounded-lg mb-2 flex items-center py-2"
        v-if="signet.info"
      >
        <div class="px-2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-8 w-8 text-white"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
            />
          </svg>
        </div>
        <span v-text="signet.info" />
      </div>
      <table class="table-auto w-full mt-2">
        <thead>
          <tr class="uppercase bg-gray-300 dark:bg-gray-800 dark:text-gray-100">
            <th class="border border-slate-600 py-2">Signet</th>
            <th class="border border-slate-600 py-2">Priority</th>
          </tr>
        </thead>
        <tr v-for="(signet, index) in signet.lists" :key="index">
          <td class="border border-slate-600 dark:text-white">
            <div class="flex flex-col px-4 py-2">
              <span
                class="font-semibold underline text-base"
                v-text="signet.name"
              />
              <span class="text-sm text-gray-600 dark:text-gray-400" v-text="signet.desc" />
            </div>
          </td>
          <td class="border border-slate-600 dark:text-white text-center">
            <span
              v-text="signet.priority"
              :class="
                ['YES', 'Start', 'CORE'].includes(signet.priority)
                  ? 'font-bold'
                  : ''
              "
            />
          </td>
        </tr>
      </table>
    </DisclosurePanel>
  </Disclosure>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from "@headlessui/vue";
import { ChevronUpIcon } from "@heroicons/vue/solid";

defineProps({
  signet: Object,
});
</script>
