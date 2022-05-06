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
    <div v-for="(supp, index) in support" :key="index">
      <DisclosurePanel class="px-4 text-sm flex bg-white">
        <div
          class="
            grow
            border border-indigo-600
            text-center
            font-semibold
            flex
            justify-between
          "
        >
          <div class="border border-indigo-600 w-12 lg:w-16 py-2">
            <span v-text="supp.time" />
          </div>
          <div class="border border-indigo-600 grow py-2">
            <span v-text="supp.sigils" />
          </div>
          <div class="border border-indigo-600 w-10 lg:w-16 py-2">
            <span v-text="supp.support_1" />
          </div>
          <div class="border border-indigo-600 w-10 lg:w-16 py-2">
            <span v-text="supp.support_2" />
          </div>
        </div>
      </DisclosurePanel>
    </div>
  </Disclosure>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from "@headlessui/vue";
import { ChevronUpIcon } from "@heroicons/vue/solid";

defineProps({
  support: Array,
});
</script>
