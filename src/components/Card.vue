<template>
	<a class="group" @click="open = true">
		<div class="border border-white w-full aspect-w-1 aspect-h-1 bg-gray-200 rounded-tr-[30px] overflow-hidden xl:aspect-w-7 xl:aspect-h-8 group-hover:rounded-none">
			<img :src="valkyrie.imageSrc" :alt="valkyrie.imageAlt" class="w-full h-full object-cover group-hover:opacity-75 transtition-transform ease-in-out duration-500 transform group-hover:scale-110" :class="valkyrie.position" />
		</div>
		<h3 class="border border-white text-sm bg-gradient-to-r from-pink-500 via-purple-600 to-violet-800 group-hover:from-pink-400 group-hover:via-purple-500 group-hover:to-violet-700 rounded-bl-[30px] px-4 py-3 uppercase text-white font-semibold group-hover:font-bold group-hover:rounded-none">
			<p class="transform ml-4 group-hover:translate-x-3 transition-transform ease-in-out duration-500">{{ valkyrie.name }}</p>
		</h3>
	</a>
  <TransitionRoot as="template" :show="open" :id="valkyrie.id">
    <Dialog as="div" class="fixed inset-0 overflow-hidden" @close="open = false" :id="valkyrie.id">
      <div class="absolute inset-0 overflow-hidden">
        <TransitionChild as="template" enter="ease-in-out duration-500" enter-from="opacity-0" enter-to="opacity-100" leave="ease-in-out duration-500" leave-from="opacity-100" leave-to="opacity-0">
          <DialogOverlay class="absolute inset-0 bg-gray-500 bg-opacity-75 transition-opacity" />
        </TransitionChild>
        <div class="pointer-events-none fixed inset-y-0 right-0 flex max-w-full pl-10">
          <TransitionChild as="template" enter="transform transition ease-in-out duration-500 sm:duration-700" enter-from="translate-x-full" enter-to="translate-x-0" leave="transform transition ease-in-out duration-500 sm:duration-700" leave-from="translate-x-0" leave-to="translate-x-full">
            <div class="pointer-events-auto relative w-screen">
              <TransitionChild as="template" enter="ease-in-out duration-500" enter-from="opacity-0" enter-to="opacity-100" leave="ease-in-out duration-500" leave-from="opacity-100" leave-to="opacity-0">
                <div class="absolute top-0 left-0 -ml-8 flex pt-4 pr-2 sm:-ml-10 sm:pr-4">
                  <button type="button" class="rounded-md text-gray-300 hover:text-white focus:outline-none focus:ring-2 focus:ring-white" @click="open = false">
                    <span class="sr-only">Close panel</span>
                    <XIcon class="h-6 w-6" aria-hidden="true" />
                  </button>
                </div>
              </TransitionChild>
              <div class="flex h-full flex-col overflow-y-scroll bg-gradient-to-br from-fuchsia-500 via-violet-600 to-purple-500 py-6 shadow-xl">
                <div class="px-4 sm:px-6">
                  <DialogTitle class="text-lg font-semibold text-white uppercase"> {{ valkyrie.name }} </DialogTitle>
                </div>
                <div class="relative mt-6 flex-1 px-4 sm:px-6">
                  <!-- Replace with your content -->
                  <div class="absolute inset-0 px-4 sm:px-6">
                    <div class="w-full px-2 py-4 sm:px-0">
                      <div class="w-full px-4 space-y-3">
                        <div class="w-full p-2 mx-auto bg-gray-100 rounded-2xl">
                          <TabGroup>
                            <TabList class="flex p-1 space-x-1 bg-gradient-to-r from-pink-500 via-fuchsia-600 to-purple-700 rounded-xl">
                              <Tab
                                v-for="signet in signets.builds"
                                as="template"
                                :key="signet.id"
                                v-slot="{ selected }"
                              >
                                <button
                                  :class="[
                                    'w-full py-2.5 text-sm leading-5 font-medium rounded-lg',
                                    'focus:outline-none focus:ring-2 ring-offset-2 ring-offset-blue-400 ring-white ring-opacity-60',
                                    selected
                                      ? 'bg-white text-blue-700'
                                      : 'text-white',
                                  ]"
                                >
                                  {{ signet.name }}
                                </button>
                              </Tab>
                            </TabList>

                            <TabPanels class="mt-2">
                              <TabPanel
                                v-for="signet in signets.builds"
                                :key="signet"
                                :class="[
                                  'bg-white rounded-xl p-3',
                                  'focus:outline-none focus:ring-2 ring-offset-2 ring-offset-blue-400 ring-white ring-opacity-60',
                                ]"
                              >
                                <div
                                  v-for="sign in signet.signets"
                                  :key="sign.id"
                                  class="relative p-3 rounded-md"
                                >
                                  <Signet :signet="sign" />
                                </div>
                              </TabPanel>
                            </TabPanels>
                          </TabGroup>
                        </div>
                      </div>
                    </div>
                  </div>
                  <!-- /End replace -->
                </div>
              </div>
            </div>
          </TransitionChild>
        </div>
      </div>
    </Dialog>
  </TransitionRoot>
</template>

<script setup>
import Signet from './Signet.vue'
import { ref } from 'vue'
import { XIcon } from '@heroicons/vue/outline'
import { TabGroup, TabList, TabPanel, Tab, Dialog, DialogOverlay, DialogTitle, TransitionChild, TransitionRoot } from '@headlessui/vue'

defineProps({
  valkyrie: Object,
  signets: Object
});

const open = ref(false)
</script>