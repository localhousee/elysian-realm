<template>
  <div>
    <h1 class="
        text-center
        uppercase
        font-thin
        text-[60px]
        tracking-widest
        pb-10
        text-slate-900
        dark:text-white
      ">
      Elysian Realm
    </h1>
    <div class="flex justify-center space-x-4">
      <Modal>
        <template #title><svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" fill="none" viewBox="0 0 24 24"
            stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round"
              d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
          </svg>
          About</template>
        <div class="
            mt-2
            text-sm
            lg:text-md
            text-gray-800
            dark:text-white
            mx-4
            space-y-2
          ">
          <p>
            This page created by
            <a target="_blank" class="
                text-blue-500
                dark:text-blue-400
                font-semibold
                underline
                hover:text-blue-400
                dark:hover:text-blue-500
              " href="https://github.com/localhousee">me</a>
          </p>
          <p>
            Say Thanks to
            <a class="
                text-blue-500
                dark:text-blue-400
                underline
                font-semibold
                hover:text-blue-400
                dark:hover:text-blue-500
              " target="_blank"
              href="https://github.com/localhousee/elysian-realm/blob/main/README.md#kudos-to-these-heroes-">these
              heroes</a>. I can't do much without them
          </p>
          <p>
            If you want to improve this website, make sure to check
            <a class="
                text-blue-500
                dark:text-blue-400
                underline
                font-semibold
                hover:text-blue-400
                dark:hover:text-blue-500
              " target="_blank" href="https://github.com/localhousee/elysian-realm/blob/main/README.md#faq">this</a>
          </p>
          <p>
            Source for each pic goes
            <a class="
                text-blue-500
                dark:text-blue-400
                underline
                font-semibold
                hover:text-blue-400
                dark:hover:text-blue-500
              " target="_blank"
              href="https://github.com/localhousee/elysian-realm/blob/main/README.md#credits-%EF%B8%8F">here</a>
          </p>
        </div>
      </Modal>
      <Modal>
        <template #title><svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" fill="none" viewBox="0 0 24 24"
            stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round"
              d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z" />
            <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
          </svg>Settings</template>
        <div class="
            mt-8
            text-sm
            lg:text-md
            text-gray-800
            dark:text-white
            mx-4
            space-y-4
            flex
            flex-col
          ">
          <div class="flex justify-between">
            <label>Dark Mode</label>
            <SwitchGroup>
              <Switch v-model="isDarkMode" :class="isDarkMode ? 'bg-gray-800' : 'bg-gray-200'" class="
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
                ">
                <span :class="isDarkMode ? 'translate-x-6' : 'translate-x-1'" class="
                    inline-block
                    h-4
                    w-4
                    transform
                    rounded-full
                    bg-white
                    transition-transform
                  " />
              </Switch>
            </SwitchGroup>
          </div>
          <div class="flex justify-between">
            <div class="flex flex-col">
              <label>Derp Mode</label>
              <span class="text-xs text-red-500 dark:text-rose-500">Some Valks may not change to Derp Mode</span>
            </div>
            <SwitchGroup>
              <Switch v-model="isDerpMode" :class="isDerpMode ? 'bg-gray-800' : 'bg-gray-200'" class="
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
                ">
                <span :class="isDerpMode ? 'translate-x-6' : 'translate-x-1'" class="
                    inline-block
                    h-4
                    w-4
                    transform
                    rounded-full
                    bg-white
                    transition-transform
                  " />
              </Switch>
            </SwitchGroup>
          </div>
        </div>
      </Modal>
      <a href="https://rentry.org/hi3er" target="_blank" class="
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
        ">
        <span class="flex">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" fill="none" viewBox="0 0 24 24"
            stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round"
              d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9" />
          </svg>
          Rentry link
        </span>
      </a>
    </div>
    <div class="flex justify-center mt-10 px-8">
      <input type="text" v-model="query" placeholder="Search for Valkyrie ..." class="
          bg-gray-200
          dark:bg-slate-700 dark:text-slate-100
          px-8
          py-2
          w-full
          max-w-lg
          border-none
          rounded-full
          caret-slate-800
          placeholder-slate-500
          dark:caret-slate-300 dark:shadow-slate-800 dark:placeholder-slate-500
          focus:outline-none focus:ring-0
          shadow-lg
        " />
    </div>
    <div class="max-w-2xl mx-auto py-10 px-4 sm:py-24 sm:px-6 lg:max-w-7xl lg:px-8">
      <div class="
          gap-y-10 gap-x-6
          grid grid-cols-2
          md:grid-cols-4
          lg:grid-cols-5
          xl:gap-x-8
        ">
        <ArgentKnightArtemis :key="key" v-if="'argent knight artemis rita aka'.includes(query)" />
        <BrightKnightExcelsis :key="key" v-if="'durandal bright knight excelsis dudu bkek'.includes(query)" />
        <DeaAnchora :key="key" v-if="'durandal dea anchora dudu da'.includes(query)" />
        <DisciplinaryPerdition :key="key" v-if="'disciplinary perdition aponia dpe dip'.includes(query)" />
        <FallenRosemary :key="key" v-if="'fr fallen rosemary rita'.includes(query)" />
        <FerventTempo :key="key" v-if="'ft fervent tempo rozaliya'.includes(query)" />
        <GoldenDiva :key="key" v-if="'golden diva eden gd'.includes(query)" />
        <HerrscherOfFlamescion :key="key" v-if="'herrscher of flamescion hofs hfs fk kiana'.includes(query)" />
        <HerrscherOfReason :key="key" v-if="'herrscher of reason hor hr bronya'.includes(query)" />
        <HerrscherOfSentience :key="key" v-if="
          'herrscher of sentience hos hs fuhua fu hua fuka'.includes(query)
        " />
        <HerrscherOfThunder :key="key" v-if="'herrscher of thunder hot ht mei'.includes(query)" />
        <InfiniteOuroboros :key="key" v-if="'infinite ouroboros mobius io'.includes(query)" />
        <LunaKindred :key="key" v-if="'teri-teri teriri luna kindred lk theresa'.includes(query)" />
        <MidnightAbsinthe :key="key" v-if="'midnight absinthe raven ma'.includes(query)" />
        <MissPinkElf :key="key" v-if="'miss pink elf elysia mpe'.includes(query)" />
        <PalatinusEquinox :key="key" v-if="'durandal palatinus equinox pe dudu juan'.includes(query)" />
        <PrinzessinDerVerurteilung :key="key" v-if="'prinzessin der verurteilung pv fish fischl'.includes(query)" />
        <ReveristCalico :key="key" v-if="'reverist calico cat neko rc pardofelis'.includes(query)" />
        <RitualImayoh :key="key" v-if="'ritual imayoh kallen ir'.includes(query)" />
        <SilverwingNEX :key="key" v-if="'silverwing nex bronya n-ex sw'.includes(query)" />
        <SpinaAstera :key="key" v-if="'spina astera spa rita'.includes(query)" />
        <StarchasmNyx :key="key" v-if="'starchasm nyx seele'.includes(query)" />
        <StarryImpression :key="key" v-if="'griseo starry impression'.includes(query)" />
        <StrikerFulminata :key="key" v-if="'striker fulminata mei stfu'.includes(query)" />
        <StygianNymph :key="key" v-if="'stygnian nymph seele sn'.includes(query)" />
        <SweetNSpicy :key="key" v-if="'sweet n spicy carole sns'.includes(query)" />
        <TwilightPaladin :key="key" v-if="'teri-teri teriri twilight paladin tp theresa'.includes(query)" />
        <ValkyrieGloria :key="key" v-if="'durandal valkyrie gloria vg dudu'.includes(query)" />
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, watchEffect } from "vue";
import { Switch, SwitchGroup, SwitchLabel } from "@headlessui/vue";
import Modal from "../components/Modal.vue";
import ArgentKnightArtemis from "./Valkyries/ArgentKnightArtemis.vue";
import BrightKnightExcelsis from "./Valkyries/BrightKnightExcelsis.vue";
import DeaAnchora from "./Valkyries/DeaAnchora.vue";
import DisciplinaryPerdition from "./Valkyries/DisciplinaryPerdition.vue";
import FallenRosemary from "./Valkyries/FallenRosemary.vue";
import FerventTempo from "./Valkyries/FerventTempo.vue";
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
import StarryImpression from "./Valkyries/StarryImpression.vue";
import StrikerFulminata from "./Valkyries/StrikerFulminata.vue";
import StygianNymph from "./Valkyries/StygianNymph.vue";
import SweetNSpicy from "./Valkyries/SweetNSpicy.vue";
import TwilightPaladin from "./Valkyries/TwilightPaladin.vue";
import ValkyrieGloria from "./Valkyries/ValkyrieGloria.vue";

let query = ref("");

let theme = ref(window.localStorage.getItem('theme'));
let derp = ref(window.localStorage.getItem('derp'));

let isDerpMode = ref(derp.value === "derp" ? true : false);
let isDarkMode = ref(theme.value === "dark" ? true : false);
let html = document.getElementById("theme");
let body = document.getElementById("derp");
let key = ref(Number.MIN_SAFE_INTEGER);

watchEffect(() => {
  if (query.value.length > 0) {
    query.value = query.value.toLowerCase();
  }

  if (isDarkMode.value) {
    theme.value = "dark";
    window.localStorage.setItem("theme", "dark");
    html.setAttribute("class", "dark");
  } else {
    theme.value = false;
    window.localStorage.removeItem("theme");
    html.removeAttribute("class");
  }

  if (isDerpMode.value) {
    derp.value = "derp";
    window.localStorage.setItem("derp", "derp");
    body.setAttribute("derp-data", "derp");
    key.value++;
  } else {
    derp.value = false;
    window.localStorage.removeItem("derp");
    body.removeAttribute("derp-data");
    key.value++;
  }
});
</script>
