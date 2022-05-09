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
      <span>Supports</span>
      <ChevronUpIcon
        :class="open ? 'transform rotate-180' : ''"
        class="w-5 h-5 text-purple-500"
      />
    </DisclosureButton>
      <DisclosurePanel class="px-4 text-sm flex bg-white">
        <table class="table-auto w-full">
          <thead>
            <tr class="uppercase">
              <th class="border border-indigo-600">Time</th>
              <th class="border border-indigo-600">Sigils</th>
              <th class="border border-indigo-600" colspan="2">Supports</th>
            </tr>
          </thead>
          <tbody>
          <tr class="text-center" v-for="(supp, index) in support" :key="index">
            <td class="py-1 border border-indigo-600 w-12">
            <span v-text="supp.time" />
            </td>
            <td class="py-1 border border-indigo-600">
            <span v-text="supp.sigils" />
            </td>
            <td class="py-1 border border-indigo-600 w-16 font-semibold">
            <span v-text="supp.support_1" />
            </td>
            <td class="py-1 border border-indigo-600 w-16 font-semibold">
            <span v-text="supp.support_2" />
            </td>
          </tr>
          </tbody>
        </table>
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
