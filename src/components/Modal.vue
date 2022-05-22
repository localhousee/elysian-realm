<template>
  <button
    type="button"
    @click="toggle"
    class="
      pl-2
      pr-4
      py-2
      text-sm
      font-medium
      text-white
      bg-gray-900
      hover:bg-gray-700
      dark:bg-cyan-600 dark:hover:bg-cyan-500
      rounded-md
      focus:outline-none
      focus-visible:ring-2
      focus-visible:ring-white
      focus-visible:ring-opacity-75
    "
  >
    <span class="flex"><slot name="title" /></span>
  </button>
  <TransitionRoot appear :show="isOpen" as="template">
    <Dialog as="div" @close="toggle">
      <div class="fixed inset-0 z-10 overflow-y-auto">
        <div class="min-h-screen px-4 text-center">
          <TransitionChild
            as="template"
            enter="duration-300 ease-out"
            enter-from="opacity-0"
            enter-to="opacity-100"
            leave="duration-200 ease-in"
            leave-from="opacity-100"
            leave-to="opacity-0"
          >
            <DialogOverlay
              class="fixed inset-0 bg-gray-500 bg-opacity-75 transition-opacity"
            />
          </TransitionChild>
          <span class="inline-block h-screen align-middle" aria-hidden="true">
            &#8203;
          </span>
          <TransitionChild
            as="template"
            enter="duration-300 ease-out"
            enter-from="opacity-0 scale-95"
            enter-to="opacity-100 scale-100"
            leave="duration-200 ease-in"
            leave-from="opacity-100 scale-100"
            leave-to="opacity-0 scale-95"
          >
            <div
              class="
                inline-block
                w-full
                max-w-md
                p-6
                my-8
                overflow-hidden
                text-left
                align-middle
                transition-all
                transform
                bg-white
                dark:bg-slate-700
                shadow-xl
                rounded-2xl
              "
            >
              <DialogTitle
                as="h3"
                class="
                  text-lg
                  font-semibold
                  uppercase
                  leading-6
                  text-slate-900
                  dark:text-white
                "
              >
                <span class="flex">
                  <slot name="title" />
                </span>
              </DialogTitle>
              <slot />
              <div class="mt-4">
                <button
                  type="button"
                  class="
                    inline-flex
                    justify-center
                    px-4
                    py-2
                    text-sm
                    font-medium
                    bg-slate-900
                    text-white
                    dark:text-white dark:bg-cyan-500 dark:hover:bg-cyan-400
                    rounded-md
                    focus:outline-none
                    focus-visible:ring-2 focus-visible:ring-offset-2
                  "
                  @click="toggle"
                >
                  Close
                </button>
              </div>
            </div>
          </TransitionChild>
        </div>
      </div>
    </Dialog>
  </TransitionRoot>
</template>

<script setup>
import { ref } from "vue";
import {
  TransitionRoot,
  TransitionChild,
  Dialog,
  DialogOverlay,
  DialogTitle,
} from "@headlessui/vue";

let isOpen = ref(false);

const toggle = () => {
  isOpen.value = !isOpen.value;
};
</script>