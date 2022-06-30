<template>
  <a class="group z-0" @click="open = true">
    <div class="
        w-full
        bg-gray-200
        rounded-tr-[30px]
        overflow-hidden
        aspect-w-7 aspect-h-8
        group-hover:rounded-none
        cursor-pointer
      ">
      <img v-if="derpMode" loading="lazy" :src="valkyrie.derp?.imageSrc" :alt="valkyrie.derp?.imageAlt" class="
          w-full
          h-full
          object-cover
          transtition-transform
          ease-in-out
          duration-500
          transform
          group-hover:scale-110
        " :class="valkyrie.position" />
      <img v-else loading="lazy" :src="valkyrie.imageSrc" :alt="valkyrie.imageAlt" class="
          w-full
          h-full
          object-cover
          transtition-transform
          ease-in-out
          duration-500
          transform
          group-hover:scale-110
        " :class="valkyrie.position" />
    </div>
    <h3 class="
        bg-slate-900
        group-hover:bg-slate-700
        dark:bg-cyan-600
        dark:group-hover:bg-cyan-500
        rounded-bl-[30px]
        px-4
        py-3
        uppercase
        text-white
        font-semibold
        group-hover:font-bold group-hover:rounded-none
        text-xs
      ">
      <p class="
          transform
          ml-4
          group-hover:translate-x-2
          transition-transform
          ease-in-out
          duration-500
        ">
        {{ valkyrie.name }}
      </p>
    </h3>
  </a>

  <TransitionRoot as="template" :show="open" :id="valkyrie.id">
    <Dialog as="div" class="fixed inset-0 overflow-hidden" @close="open = false" :id="valkyrie.id">
      <div class="absolute inset-0 overflow-hidden">
        <TransitionChild as="template" enter="ease-in-out duration-500" enter-from="opacity-0" enter-to="opacity-100"
          leave="ease-in-out duration-500" leave-from="opacity-100" leave-to="opacity-0">
          <DialogOverlay class="
              absolute
              inset-0
              bg-gray-500 bg-opacity-75
              transition-opacity
            " />
        </TransitionChild>
        <div class="
            pointer-events-none
            fixed
            inset-y-0
            right-0
            flex
            max-w-full
            pl-10
          ">
          <TransitionChild as="template" enter="transform transition ease-in-out duration-500 sm:duration-700"
            enter-from="translate-x-full" enter-to="translate-x-0"
            leave="transform transition ease-in-out duration-500 sm:duration-700" leave-from="translate-x-0"
            leave-to="translate-x-full">
            <DialogPanel class="pointer-events-auto relative w-screen lg:max-w-xl">
              <TransitionChild as="template" enter="ease-in-out duration-500" enter-from="opacity-0"
                enter-to="opacity-100" leave="ease-in-out duration-500" leave-from="opacity-100" leave-to="opacity-0">
                <div class="
                    absolute
                    top-0
                    left-0
                    -ml-8
                    flex
                    pt-4
                    pr-2
                    sm:-ml-10 sm:pr-4
                  ">
                  <button type="button" class="
                      rounded-md
                      text-gray-300
                      hover:text-white
                      focus:outline-none focus:ring-2 focus:ring-white
                    " @click="open = false">
                    <span class="sr-only">Close panel</span>
                    <XIcon class="h-6 w-6" aria-hidden="true" />
                  </button>
                </div>
              </TransitionChild>
              <div class="
                  flex
                  h-full
                  flex-col
                  overflow-y-scroll
                  bg-gray-100
                  dark:bg-slate-900
                  py-6
                  shadow-xl
                ">
                <div class="px-4 sm:px-6">
                  <DialogTitle class="text-lg font-semibold text-slate-900 dark:text-white uppercase">
                    {{ valkyrie.name }}
                  </DialogTitle>
                </div>
                <div class="relative mt-6 flex-1 px-4 sm:px-6">
                  <!-- Replace with your content -->
                  <div class="absolute inset-0 px-4 sm:px-6">
                    <div class="w-full px-2 py-4 sm:px-0">
                      <div class="w-full px-4 space-y-3">
                        <div class="w-full p-2 mx-auto bg-gray-100 dark:bg-slate-900 rounded-2xl">
                          <Tabs :signets="signets" />
                        </div>
                      </div>
                    </div>
                  </div>
                  <!-- /End replace -->
                </div>
              </div>
            </DialogPanel>
          </TransitionChild>
        </div>
      </div>
    </Dialog>
  </TransitionRoot>
</template>

<script setup>
import { ref, watchEffect } from "vue";
import { Dialog, DialogOverlay, DialogPanel, DialogTitle, TransitionChild, TransitionRoot } from '@headlessui/vue'
import { XIcon } from '@heroicons/vue/outline'
import Tabs from './Tabs.vue'

defineProps({
  valkyrie: Object,
  signets: Object,
});

const open = ref(false);
let derpMode = ref(false);
let derp = document.getElementById('derp');

watchEffect(() => {
  if (derp.hasAttribute('derp-data')) {
    derpMode.value = true;
  } else {
    derpMode.value = false;
  }
});
</script>
