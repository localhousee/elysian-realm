<template>
  <h1 class="text-center uppercase font-thin text-[60px] tracking-widest pb-10">Elysian Realm</h1>
  <div class="flex justify-center space-x-4">
  <div>
    <button
      type="button"
      @click="openModal"
      class="px-4 py-2 text-sm font-medium text-white bg-black rounded-md bg-opacity-20 hover:bg-opacity-30 focus:outline-none focus-visible:ring-2 focus-visible:ring-white focus-visible:ring-opacity-75"
    >
      About
    </button>
    <TransitionRoot appear :show="isOpen" as="template">
      <Dialog as="div" @close="closeModal">
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
              <DialogOverlay class="fixed inset-0 bg-gray-500 bg-opacity-75 transition-opacity" />
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
                class="inline-block w-full max-w-md p-6 my-8 overflow-hidden text-left align-middle transition-all transform bg-white shadow-xl rounded-2xl"
              >
                <DialogTitle
                  as="h3"
                  class="text-lg font-medium leading-6 text-gray-900"
                >
                  About
                </DialogTitle>
                <div class="mt-2">
                  <p class="text-sm text-gray-500">
                    This Page made with love by ******
                  </p>
                </div>

                <div class="mt-4">
                  <button
                    type="button"
                    class="inline-flex justify-center px-4 py-2 text-sm font-medium text-blue-900 bg-blue-100 border border-transparent rounded-md hover:bg-blue-200 focus:outline-none focus-visible:ring-2 focus-visible:ring-offset-2 focus-visible:ring-blue-500"
                    @click="closeModal"
                  >
                    Got it, thanks!
                  </button>
                </div>
              </div>
            </TransitionChild>
          </div>
        </div>
      </Dialog>
    </TransitionRoot>
  </div>
  <a href="https://rentry.org/hi3er" target="_blank" class="px-4 py-2 text-sm font-medium text-white bg-black rounded-md bg-opacity-20 hover:bg-opacity-30 focus:outline-none focus-visible:ring-2 focus-visible:ring-white focus-visible:ring-opacity-75">Rentry link</a>
  </div>
  <div class="max-w-2xl mx-auto py-10 px-4 sm:py-24 sm:px-6 lg:max-w-7xl lg:px-8">
    <div class="grid grid-cols-1 gap-y-10 sm:grid-cols-2 gap-x-6 lg:grid-cols-4 xl:gap-x-8">
      <ArgentKnightArtemis />
      <BrightKnightExcelsis />
      <DeaAnchora />
      <FallenRosemary />
      <HerrscherOfFlamescion />
      <HerrscherOfReason />
      <HerrscherOfSentience />
      <HerrscherOfThunder />
      <InfiniteOuroboros />
      <LunaKindred />
      <MidnightAbsinthe />
      <MissPinkElf />
      <PalatinusEquinox />
      <PrinzessinDerVerurteilung />
      <ReveristCalico />
      <RitualImayoh />
      <SilverwingNEX />
      <SpinaAstera />
      <StarchasmNyx />
      <StrikerFulminata />
      <StygianNymph />
      <SweetNSpicy />
      <TwilightPaladin />
      <ValkyrieGloria />
    </div>
  </div>
</template>

<script setup>
  import { ref } from 'vue'
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue'

  import { TransitionRoot, TransitionChild, Dialog, DialogOverlay, DialogTitle } from '@headlessui/vue'
  import ArgentKnightArtemis from './Valkyries/ArgentKnightArtemis.vue';
  import BrightKnightExcelsis from './Valkyries/BrightKnightExcelsis.vue';
  import DeaAnchora from './Valkyries/DeaAnchora.vue';
  import FallenRosemary from './Valkyries/FallenRosemary.vue';
  import HerrscherOfFlamescion from './Valkyries/HerrscherOfFlamescion.vue';
  import HerrscherOfReason from './Valkyries/HerrscherOfReason.vue';
  import HerrscherOfSentience from './Valkyries/HerrscherOfSentience.vue';
  import HerrscherOfThunder from './Valkyries/HerrscherOfThunder.vue';
  import InfiniteOuroboros from './Valkyries/InfiniteOuroboros.vue';
  import LunaKindred from './Valkyries/LunaKindred.vue';
  import MidnightAbsinthe from './Valkyries/MidnightAbsinthe.vue';
  import PalatinusEquinox from './Valkyries/PalatinusEquinox.vue';
  import ReveristCalico from './Valkyries/ReveristCalico.vue';
  import RitualImayoh from './Valkyries/RitualImayoh.vue';
  import MissPinkElf from './Valkyries/MissPinkElf.vue';
  import PrinzessinDerVerurteilung from './Valkyries/PrinzessinDerVerurteilung.vue';
  import SilverwingNEX from './Valkyries/SilverwingNEX.vue';
  import SpinaAstera from './Valkyries/SpinaAstera.vue';
  import StarchasmNyx from './Valkyries/StarchasmNyx.vue';
  import StrikerFulminata from './Valkyries/StrikerFulminata.vue';
  import StygianNymph from './Valkyries/StygianNymph.vue';
  import SweetNSpicy from './Valkyries/SweetNSpicy.vue';
  import TwilightPaladin from './Valkyries/TwilightPaladin.vue';
  import ValkyrieGloria from './Valkyries/ValkyrieGloria.vue';

  const isOpen = ref(false)

  function closeModal() {
    isOpen.value = false
  }
  function openModal() {
    isOpen.value = true
  }

const categories = ref({
  Recent: [
    {
      id: 1,
      title: 'Does drinking coffee make you smarter?',
      date: '5h ago',
      commentCount: 5,
      shareCount: 2,
    },
    {
      id: 2,
      title: "So you've bought coffee... now what?",
      date: '2h ago',
      commentCount: 3,
      shareCount: 2,
    },
  ],
  Popular: [
    {
      id: 1,
      title: 'Is tech making coffee better or worse?',
      date: 'Jan 7',
      commentCount: 29,
      shareCount: 16,
    },
    {
      id: 2,
      title: 'The most innovative things happening in coffee',
      date: 'Mar 19',
      commentCount: 24,
      shareCount: 12,
    },
  ],
  Trending: [
    {
      id: 1,
      title: 'Ask Me Anything: 10 answers to your questions about coffee',
      date: '2d ago',
      commentCount: 9,
      shareCount: 5,
    },
    {
      id: 2,
      title: "The worst advice we've ever heard about coffee",
      date: '4d ago',
      commentCount: 1,
      shareCount: 2,
    },
  ],
})
</script>
