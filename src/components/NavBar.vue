<template>
  <Disclosure as="nav" v-slot="{ open }">
    <div class="mx-auto max-w-7xl px-2 lg:px-6 lg:px-8" style="position: fixed; z-index: 1; cursor: pointer;">
      <div class="relative flex h-16 justify-between ml-20">
        <div class="absolute inset-y-0 left-0 flex items-center nx:hidden">
          <!-- Mobile menu button-->
          <DisclosureButton class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white">
            <span class="absolute -inset-0.5" />
            <span class="sr-only">Open main menu</span>
            <Bars3Icon v-if="!open" class="block h-6 w-6" aria-hidden="true" />
            <XMarkIcon v-else class="block h-6 w-6" aria-hidden="true" />
          </DisclosureButton>
        </div>
        <div class="flex flex-1 lg:items-stretch lg:justify-start">
          <div class="hidden nx:ml-6 nx:block">
            <div class="flex space-x-4" style="text-shadow: 2px 2px 4px rgba(0, 0, 0);">
              <a v-for="item in navigation" :key="item.name" v-scroll-to="item.href" :class="[item.current ? 'bg-[#be61c0] text-white hover:bg-[#6d256e] font-bold' : 'text-gray-300 hover:bg-[#6d256e]', 'rounded-sm px-3 py-2 text-lg font-bold drop-shadow-xl']" :aria-current="item.current ? 'page' : undefined">{{ item.name }} </a>
            </div>
          </div>
        </div>
      </div>
    </div>

    <DisclosurePanel class="lg:hidden">
      <div class="space-y-1 px-2 pb-3 pt-2">
        <DisclosureButton v-for="item in navigation" :key="item.name" as="a" v-scroll-to="item.href" :class="[item.current ? 'bg-[#be61c0] text-white hover:bg-[#6d256e]' : 'text-gray-300 hover:bg-[#6d256e] hover:text-white', 'block rounded-sm px-3 py-2 text-base font-medium']" :aria-current="item.current ? 'page' : undefined">{{ item.name }}</DisclosureButton>
      </div>
    </DisclosurePanel>
  </Disclosure>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from '@headlessui/vue';
import { Bars3Icon, XMarkIcon } from '@heroicons/vue/24/outline';

const navigation = [
  { name: 'Início', href: '#start-screen', current: false },
  { name: 'Sobre mim', href: '#about-me', current: false },
  { name: 'Projetos', href: '#projects', current: false },
  { name: 'Experiências', href: '#experience', current: false },
  { name: 'Depoimento', href: '#testimony', current: false },
  { name: 'Contatos', href: '#contacts', current: true },
];
</script>
