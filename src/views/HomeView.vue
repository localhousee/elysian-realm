<template>
  <div>
    <h1
      class="
        text-center
        uppercase
        font-thin
        text-[60px]
        tracking-widest
        pb-10
        text-slate-900
        dark:text-white
      "
    >
      Elysian Realm
    </h1>
    <div class="flex justify-center space-x-4">
      <Modal>
        <template #title
          ><svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6 mr-2"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
            />
          </svg>
          About</template
        >
        <div
          class="
            mt-2
            text-sm
            lg:text-md
            text-gray-800
            dark:text-white
            mx-4
            space-y-2
          "
        >
          <p>
            This page created by
            <a
              target="_blank"
              class="
                text-blue-500
                dark:text-blue-400
                font-semibold
                underline
                hover:text-blue-400
                dark:hover:text-blue-500
              "
              href="https://github.com/localhousee"
              >me</a
            >
          </p>
          <p>
            Say Thanks to
            <a
              class="
                text-blue-500
                dark:text-blue-400
                underline
                font-semibold
                hover:text-blue-400
                dark:hover:text-blue-500
              "
              target="_blank"
              href="https://github.com/localhousee/elysian-realm/blob/main/README.md#kudos-to-these-heroes-"
              >these heroes</a
            >. I can't do much without them
          </p>
          <p>
            If you want to improve this website, make sure to check
            <a
              class="
                text-blue-500
                dark:text-blue-400
                underline
                font-semibold
                hover:text-blue-400
                dark:hover:text-blue-500
              "
              target="_blank"
              href="https://github.com/localhousee/elysian-realm/blob/main/README.md#faq"
              >this</a
            >
          </p>
          <p>
            Source for each pic goes
            <a
              class="
                text-blue-500
                dark:text-blue-400
                underline
                font-semibold
                hover:text-blue-400
                dark:hover:text-blue-500
              "
              target="_blank"
              href="https://github.com/localhousee/elysian-realm/blob/main/README.md#credits-%EF%B8%8F"
              >here</a
            >
          </p>
        </div>
      </Modal>
      <Modal>
        <template #title
          ><svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6 mr-2"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z"
            />
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"
            /></svg
          >Settings</template
        >
        <div
          class="
            mt-8
            text-sm
            lg:text-md
            text-gray-800
            dark:text-white
            mx-4
            space-y-4
          "
        >
          <SwitchGroup>
            <div class="flex items-center">
              <SwitchLabel passive class="mr-4">Dark Mode</SwitchLabel>
              <Switch
                v-model="darkMode"
                :class="darkMode ? 'bg-gray-800' : 'bg-gray-200'"
                class="
                  relative
                  inline-flex
                  h-6
                  w-11
                  items-center
                  rounded-full
                  transition-colors
                  focus:outline-none focus:ring-2 focus:ring-slate-900
                  dark:focus:ring-slate-500
                  focus:ring-offset-2
                "
              >
                <span
                  :class="darkMode ? 'translate-x-6' : 'translate-x-1'"
                  class="
                    inline-block
                    h-4
                    w-4
                    transform
                    rounded-full
                    bg-white
                    transition-transform
                  "
                />
              </Switch>
            </div>
          </SwitchGroup>
        </div>
      </Modal>
      <a
        href="https://rentry.org/hi3er"
        target="_blank"
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
        <span class="flex">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6 mr-2"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9"
            />
          </svg>
          Rentry link
        </span>
      </a>
    </div>
    <div class="flex justify-center mt-10 px-8">
      <input
        type="text"
        v-model="query"
        placeholder="Search for Valkyrie ..."
        class="
          bg-gray-200
          dark:bg-slate-700
          dark:text-slate-100
          px-8
          py-2
          w-full
          max-w-lg
          border-none
          rounded-full
          caret-slate-800
          placeholder-slate-500
          dark:caret-slate-300
          dark:shadow-slate-800
          dark:placeholder-slate-500
          focus:outline-none focus:ring-0
          shadow-lg
        "
      />
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
        <ArgentKnightArtemis v-if="'argent knight artemis'.includes(query)" />
        <BrightKnightExcelsis v-if="'bright knight excelsis'.includes(query)" />
        <DeaAnchora v-if="'dea anchora'.includes(query)" />
        <DisciplinaryPerdition v-if="'disciplinary perdition'.includes(query)" />
        <FallenRosemary v-if="'fallen rosemary'.includes(query)" />
        <GoldenDiva v-if="'golden diva'.includes(query)" />
        <HerrscherOfFlamescion v-if="'herrscher of flamescion'.includes(query)" />
        <HerrscherOfReason v-if="'herrscher of reason'.includes(query)" />
        <HerrscherOfSentience v-if="'herrscher of sentience'.includes(query)" />
        <HerrscherOfThunder v-if="'herrscher of thunder'.includes(query)" />
        <InfiniteOuroboros v-if="'infinite ouroboros'.includes(query)" />
        <LunaKindred v-if="'luna kindred'.includes(query)" />
        <MidnightAbsinthe v-if="'midnight absinthe'.includes(query)" />
        <MissPinkElf v-if="'miss pink elf'.includes(query)" />
        <PalatinusEquinox v-if="'palatinus equinox'.includes(query)" />
        <PrinzessinDerVerurteilung v-if="'prinzessin der verurteilung'.includes(query)" />
        <ReveristCalico v-if="'reveris calico'.includes(query)" />
        <RitualImayoh v-if="'ritual imayoh'.includes(query)" />
        <SilverwingNEX v-if="'silverwing nex'.includes(query)" />
        <SpinaAstera v-if="'spina astera'.includes(query)" />
        <StarchasmNyx v-if="'starchasm nyx'.includes(query)" />
        <StrikerFulminata v-if="'striker fulminata'.includes(query)" />
        <StygianNymph v-if="'stygnian nymph'.includes(query)" />
        <SweetNSpicy v-if="'sweet n spicy'.includes(query)" />
        <TwilightPaladin v-if="'twilight paladin'.includes(query)" />
        <ValkyrieGloria v-if="'valkyrie gloria'.includes(query)" />
      </div>
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
import { Switch, SwitchGroup, SwitchLabel } from "@headlessui/vue";
import { CheckIcon, SelectorIcon } from "@heroicons/vue/solid";
import Modal from "../components/Modal.vue";
import ArgentKnightArtemis from "./Valkyries/ArgentKnightArtemis.vue";
import BrightKnightExcelsis from "./Valkyries/BrightKnightExcelsis.vue";
import DeaAnchora from "./Valkyries/DeaAnchora.vue";
import DisciplinaryPerdition from "./Valkyries/DisciplinaryPerdition.vue";
import FallenRosemary from "./Valkyries/FallenRosemary.vue";
import GoldenDiva from "./Valkyries/GoldenDiva.vue";
import HerrscherOfFlamescion from "./Valkyries/HerrscherOfFlamescion.vue";
import HerrscherOfReason from "./Valkyries/HerrscherOfReason.vue";
import HerrscherOfSentience from "./Valkyries/HerrscherOfSentience.vue";
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

const query = ref("");
</script>
