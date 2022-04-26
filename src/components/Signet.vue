<template>
  <Disclosure v-slot="{ open }" as="div">
    <DisclosureButton
      class="flex justify-between w-full px-4 py-2 text-sm font-medium text-left text-purple-900 bg-purple-100 rounded-lg hover:bg-purple-200 focus:outline-none focus-visible:ring focus-visible:ring-purple-500 focus-visible:ring-opacity-75"
    >
      <span>{{ signet.name }}</span>
      <ChevronUpIcon
        :class="open ? 'transform rotate-180' : ''"
        class="w-5 h-5 text-purple-500"
      />
    </DisclosureButton>
      <div v-for="signet in signet.lists" :key="signet.id">
        <DisclosurePanel class="px-4 pt-4 pb-2 text-sm text-gray-500 flex justify-between">
          <span v-text="signet.name" />
          <span v-text="signet.priority" />
        </DisclosurePanel>
      </div>
  </Disclosure>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from '@headlessui/vue'
import { ChevronUpIcon } from '@heroicons/vue/solid'

defineProps({
  signet: Array,
})
</script>
