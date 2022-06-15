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
      <span>Supports</span>
      <ChevronUpIcon
        :class="open ? 'transform rotate-180' : ''"
        class="w-5 h-5 text-slate-900 group-hover:text-white dark:text-white"
      />
    </DisclosureButton>
      <DisclosurePanel class="px-4 text-sm flex bg-transparent">
        <table class="table-auto w-full mt-2">
          <thead>
            <tr class="uppercase bg-gray-300 dark:bg-gray-800 dark:text-gray-100">
              <th class="border border-slate-600 py-2">Time</th>
              <th class="border border-slate-600 py-2">Sigils</th>
              <th class="border border-slate-600 py-2" colspan="2">Supports</th>
            </tr>
          </thead>
          <tbody>
          <tr class="text-center dark:text-white" v-for="(supp, index) in support" :key="index">
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
