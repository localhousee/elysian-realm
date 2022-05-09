<template>
  <Disclosure v-slot="{ open }" as="div">
    <DisclosureButton
      class="
        flex
        justify-between
        w-full
        px-4
        py-2
        text-sm
        font-medium
        text-left text-purple-900
        bg-purple-100
        rounded-lg
        hover:bg-purple-200
        focus:outline-none
        focus-visible:ring
        focus-visible:ring-purple-500
        focus-visible:ring-opacity-75
      "
    >
      <span>{{ signet.name }}</span>
      <ChevronUpIcon
        :class="open ? 'transform rotate-180' : ''"
        class="w-5 h-5 text-purple-500"
      />
    </DisclosureButton>
    <DisclosurePanel class="px-4 text-sm flex flex-col bg-white">
      <div
        class="bg-gradient-to-r from-pink-500 to-pink-600  rounded-lg mb-2 flex items-center text-white py-2"
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
      <table class="table-auto w-full">
        <thead>
          <tr class="uppercase">
            <th class="border border-indigo-600">Signet</th>
            <th class="border border-indigo-600">Priority</th>
          </tr>
        </thead>
        <tr v-for="(signet, index) in signet.lists" :key="index">
          <td class="border border-indigo-600">
            <div class="flex flex-col px-4 py-2">
              <span
                class="font-semibold underline text-base"
                v-text="signet.name"
              />
              <span class="text-sm text-gray-600" v-text="signet.desc" />
            </div>
          </td>
          <td class="border border-indigo-600 text-center">
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
  signet: Array,
});
</script>
