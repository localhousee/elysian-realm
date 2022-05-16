<template>
  <h1
    class="
      text-center
      uppercase
      font-thin
      text-[60px]
      tracking-widest
      pb-10
      text-white
    "
  >
    Elysian Realm
  </h1>
  <div class="flex justify-center space-x-4">
    <Modal>
      <template #title>About</template>
      <div class="mt-2 text-sm lg:text-md text-gray-800 mx-4 space-y-2">
        <p>
          This page created by
          <a
            target="_blank"
            class="text-blue-500 font-semibold"
            href="https://github.com/localhousee"
          >me</a>
        </p>
        <p>
          Say Thanks to
          <a
            class="text-blue-500 font-semibold"
            target="_blank"
            href="https://github.com/localhousee/elysian-realm/blob/main/README.md#kudos-to-these-heroes-"
            >these heroes</a
          >. I can't do much without them
        </p>
        <p>
          If you want to improve this website, make sure to check
          <a
            class="text-blue-500 font-semibold"
            target="_blank"
            href="https://github.com/localhousee/elysian-realm/blob/main/README.md#faq"
            >this</a
          >
        </p>
        <p>
          Source for each pic goes
          <a
            class="text-blue-500 font-semibold"
            target="_blank"
            href="https://github.com/localhousee/elysian-realm/blob/main/README.md#credits-%EF%B8%8F"
            >here</a
          >
        </p>
      </div>
    </Modal>
    <a
      href="https://rentry.org/hi3er"
      target="_blank"
      class="
        px-4
        py-2
        text-sm
        font-medium
        text-white
        bg-black
        rounded-md
        bg-opacity-20
        hover:bg-opacity-30
        focus:outline-none
        focus-visible:ring-2
        focus-visible:ring-white
        focus-visible:ring-opacity-75
      "
      >Rentry link</a
    >
  </div>
  <div
    class="max-w-2xl mx-auto py-10 px-4 sm:py-24 sm:px-6 lg:max-w-7xl lg:px-8"
  >
    <div
      class="
        grid grid-cols-1
        gap-y-10
        sm:grid-cols-2
        gap-x-6
        lg:grid-cols-4
        xl:gap-x-8
      "
    >
      <ArgentKnightArtemis />
      <BrightKnightExcelsis />
      <DeaAnchora />
      <DisciplinaryPerdition />
      <FallenRosemary />
      <FerventTempo />
      <GoldenDiva />
      <Griseo />
      <HerrscherOfFlamescion />
      <HerrscherOfReason />
      <HerrscherOfSentience />
      <HerrscherOfTheVoid />
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
import { ref } from "vue";
import {
  Combobox,
  ComboboxInput,
  ComboboxButton,
  ComboboxOptions,
  ComboboxOption,
  TransitionRoot,
} from "@headlessui/vue";
import { CheckIcon, SelectorIcon } from "@heroicons/vue/solid";
import Modal from "../components/Modal.vue";
import ArgentKnightArtemis from "./Valkyries/ArgentKnightArtemis.vue";
import BrightKnightExcelsis from "./Valkyries/BrightKnightExcelsis.vue";
import DeaAnchora from "./Valkyries/DeaAnchora.vue";
import DisciplinaryPerdition from "./Valkyries/DisciplinaryPerdition.vue";
import FallenRosemary from "./Valkyries/FallenRosemary.vue";
import FerventTempo from "./Valkyries/FerventTempo.vue";
import GoldenDiva from "./Valkyries/GoldenDiva.vue";
import Griseo from "./Valkyries/Griseo.vue";
import HerrscherOfFlamescion from "./Valkyries/HerrscherOfFlamescion.vue";
import HerrscherOfReason from "./Valkyries/HerrscherOfReason.vue";
import HerrscherOfSentience from "./Valkyries/HerrscherOfSentience.vue";
import HerrscherOfTheVoid from "./Valkyries/HerrscherOfTheVoid.vue";
import HerrscherOfThunder from "./Valkyries/HerrscherOfThunder.vue";
import InfiniteOuroboros from "./Valkyries/InfiniteOuroboros.vue";
import LunaKindred from "./Valkyries/LunaKindred.vue";
import MidnightAbsinthe from "./Valkyries/MidnightAbsinthe.vue";
import MissPinkElf from "./Valkyries/MissPinkElf.vue";
import PalatinusEquinox from "./Valkyries/PalatinusEquinox.vue";
import PrinzessinDerVerurteilung from "./Valkyries/PrinzessinDerVerurteilung.vue";
import ReveristCalico from "./Valkyries/ReveristCalico.vue";
import RitualImayoh from "./Valkyries/RitualImayoh.vue";
import SilverwingNEX from "./Valkyries/SilverwingNEX.vue";
import SpinaAstera from "./Valkyries/SpinaAstera.vue";
import StarchasmNyx from "./Valkyries/StarchasmNyx.vue";
import StrikerFulminata from "./Valkyries/StrikerFulminata.vue";
import StygianNymph from "./Valkyries/StygianNymph.vue";
import SweetNSpicy from "./Valkyries/SweetNSpicy.vue";
import TwilightPaladin from "./Valkyries/TwilightPaladin.vue";
import ValkyrieGloria from "./Valkyries/ValkyrieGloria.vue";
</script>
