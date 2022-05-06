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
      <div class="mt-2 text-sm lg:text-md text-gray-800 mx-4">
        <p>This page was made with love by the HI3 community.</p>
        <h2 class="font-semibold mt-4">Credits:</h2>
        <ul class="list-disc">
          <li>
            biribiri#3681: original Rentry person did build testing and theory
            crafting
          </li>
          <li>Butter#2252: provided data</li>
          <li>boba#8849: helped format stuff correctly and tested builds</li>
          <li>Beefyeggroll#0001: helped test builds and was in beta</li>
          <li>localhousee#7786: made the vercel website</li>
          <li>VampyHime#9207: was a beta tester and translator for beta</li>
          <li>Camelva#7085: helped with build testing and data gathering</li>
          <li>
            Rafe#5610: helped rekindled the GC again and is also a rentry/vercel
            site editor
          </li>
          <li>Starlight#9581: ER help section with story progression</li>
          <li>FrediSK#5056: helped with kalpas boss</li>
          <li>Korath#5931: kalpas boss help</li>
          <li>
            Kaga#1780 (Citrus): helped get builds out there for people to see,
            theory crafter, tester and beta tester. They are also a youtuber
          </li>
        </ul>
        <h2 class="mt-3 font-semibold">Unnamed people who helped:</h2>
        <ul class="list-disc">
          <li>KenTJY#3888: theory crafter and tester</li>
          <li>Zithr0#9800: theory crafter and tester</li>
          <li>BananaCannon#3312: tester</li>
          <li>ignihyde#4498: tester</li>
          <li>Fujinee#3002: tester</li>
          <li>Topperoonie#0484: tester</li>
          <li>
            SinsOfSeven#3164 (TencentDimepiece): tester and fellow guide maker
            <a
              class="text-blue-600 hover:underline hover:text-blue-500"
              target="_blank"
              href="https://rentry.org/elysian_realm_list"
              >Signet list here</a
            >
          </li>
          <li>
            ww#1234 (Imy): inspiration and gave the green light to make guide
          </li>
        </ul>
      </div>
    </Modal>
    <Modal>
      <template #title>Credits</template>
      <div class="mt-2">
        <span class="pb-4 font-semibold text-lg"
          >Source of each image goes here :</span
        >
        <div
          class="
            grid grid-cols-1
            md:grid-cols-2
            lg:grid-cols-4
            gap-2
            md:gap-4
            lg:gap-6
            justify-items-stretch
            content-center
          "
        >
          <Link href="https://www.pixiv.net/en/artworks/94907919"
            >Website icon</Link
          >
          <Link href="https://www.remove.bg">Remove Background</Link>
          <Link href="https://arca.live/b/hk3rd/9364261"
            >Argent Knight: Artemis</Link
          >
          <Link href="https://medibang.com/picture/sv2011190326147450004348839"
            >Bright Knight: Excelsis</Link
          >
          <Link href="https://arca.live/b/hk3rd/25348184">Dea Anchora</Link>
          <Link href="https://www.huashi6.com/draw/971767"
            >Fallen Rosemary</Link
          >
          <Link href="https://arca.live/b/hk3rd/30030448"
            >Herrscher Of Flamescion</Link
          >
          <Link href="https://ygosu.com/community/animation/273965"
            >Herrscher Of Reason</Link
          >
          <Link href="https://www.qzxiu.net/w/jxz7e8.html"
            >Herrscher Of Sentience</Link
          >
          <Link
            href="https://www.reddit.com/r/CultureImpact/comments/u0kcu0/raiden_mei"
            >Herrscher Of Thunder</Link
          >
          <Link href="https://danbooru.donmai.us/posts/5292255"
            >Infinite Ouroboros</Link
          >
          <Link href="https://www.pinterest.com/pin/578290408383512224"
            >Luna Kindred</Link
          >
          <Link href="https://www.bilibili.com/read/cv6064798"
            >Midnight Absinthe</Link
          >
          <Link href="https://www.hoyolab.com/article/700343"
            >Miss Pink Elf</Link
          >
          <Link
            href="https://libredd.it/r/houkai3rd/comments/t2j24n/durandal_by_retty9349"
            >Palatinus Equinox</Link
          >
          <Link href="https://www.morinohitos.com"
            >Prinzessin der Verurteilung</Link
          >
          <Link href="https://arca.live/b/hk3rd/48931692">Reverist Calico</Link>
          <Link href="http://reactor.cc/post/4299632">Ritual Imayoh</Link>
          <Link href="https://imgur.com/gallery/0QK3TpS">Silverwing: NEX</Link>
          <Link href="https://danbooru.donmai.us/posts/5130940"
            >Spina Astera</Link
          >
          <Link href="https://arca.live/b/replay/27887743">Starchasm Nyx</Link>
          <Link href="https://arca.live/b/hk3rd/39710366"
            >Striker Fulminata</Link
          >
          <Link href="https://wallhere.com/ru/wallpaper/1685877"
            >Stygian Nymph</Link
          >
          <Link href="https://arca.live/b/hk3rd/36130080">Sweet n Spicy</Link>
          <Link href="https://www.pixiv.net/en/artworks/77212815"
            >Twilight Paladin</Link
          >
          <Link
            href="https://honkaiimpact3.hoyoverse.com/global/en-us/news/2900"
            >Valkyrie Gloria</Link
          >
        </div>
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
  <div class="flex justify-center mt-10 px-8">
    <input
      type="text"
      v-model="query"
      placeholder="Search for Valkyrie ..."
      class="
        pl-8
        pr-4
        w-full
        max-w-lg
        border-none
        rounded-l-full
        caret-fuchsia-400
        placeholder-slate-500
        focus:outline-none focus:ring-0
      "
    />
    <button class="px-2 py-4 bg-white border-none" @click="reset">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="h-5 w-5"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        stroke-width="2"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M6 18L18 6M6 6l12 12"
        />
      </svg>
    </button>
    <button class="rounded-r-full pl-1 pr-4 py-4 bg-white border-none" @click="filter">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="h-5 w-5 text--500"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        stroke-width="2"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
        />
      </svg>
    </button>
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
import {
  Combobox,
  ComboboxInput,
  ComboboxButton,
  ComboboxOptions,
  ComboboxOption,
  TransitionRoot,
} from "@headlessui/vue";
import { CheckIcon, SelectorIcon } from "@heroicons/vue/solid";
import ArgentKnightArtemis from "./Valkyries/ArgentKnightArtemis.vue";
import BrightKnightExcelsis from "./Valkyries/BrightKnightExcelsis.vue";
import DeaAnchora from "./Valkyries/DeaAnchora.vue";
import FallenRosemary from "./Valkyries/FallenRosemary.vue";
import HerrscherOfFlamescion from "./Valkyries/HerrscherOfFlamescion.vue";
import HerrscherOfReason from "./Valkyries/HerrscherOfReason.vue";
import HerrscherOfSentience from "./Valkyries/HerrscherOfSentience.vue";
import HerrscherOfThunder from "./Valkyries/HerrscherOfThunder.vue";
import InfiniteOuroboros from "./Valkyries/InfiniteOuroboros.vue";
import LunaKindred from "./Valkyries/LunaKindred.vue";
import MidnightAbsinthe from "./Valkyries/MidnightAbsinthe.vue";
import PalatinusEquinox from "./Valkyries/PalatinusEquinox.vue";
import ReveristCalico from "./Valkyries/ReveristCalico.vue";
import RitualImayoh from "./Valkyries/RitualImayoh.vue";
import MissPinkElf from "./Valkyries/MissPinkElf.vue";
import PrinzessinDerVerurteilung from "./Valkyries/PrinzessinDerVerurteilung.vue";
import SilverwingNEX from "./Valkyries/SilverwingNEX.vue";
import SpinaAstera from "./Valkyries/SpinaAstera.vue";
import StarchasmNyx from "./Valkyries/StarchasmNyx.vue";
import StrikerFulminata from "./Valkyries/StrikerFulminata.vue";
import StygianNymph from "./Valkyries/StygianNymph.vue";
import SweetNSpicy from "./Valkyries/SweetNSpicy.vue";
import TwilightPaladin from "./Valkyries/TwilightPaladin.vue";
import ValkyrieGloria from "./Valkyries/ValkyrieGloria.vue";
import Modal from "../components/Modal.vue";
import Link from "../components/Link.vue";

import { ref } from "vue";

let query = ref("");

let reset = () => {
  query.value = "";
};

let filter = () => {
  
};
</script>
