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
        <DisclosurePanel class="px-4 text-sm flex">
            <div class="grow border border-indigo-600 border-collapse">
              <div class="flex flex-col px-4 py-2">
                <span class="font-semibold underline text-base" v-text="signet.name" />
                <span class="text-sm text-gray-600" v-text="signet.desc" />
              </div>
            </div>
            <div class="flex-none w-16 text-center border border-indigo-600 border-collapse">
              <div class="text-center">
                <span v-text="signet.priority"/>
              </div>
            </div>
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
