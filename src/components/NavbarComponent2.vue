<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
</script>
<template>
    <Navbar>
      <template #logo>
        <NavbarLogo link="https://www.google.com/" alt="Dessert logo" image-url="https://marketplace.canva.com/EAFXrQCp76w/2/0/1600w/canva-glass-cake-dome-and-macarons-peach-color-with-inscription-dessert-store-modern-brand-logo-B3Okxx96E5g.jpg">
          Dessert Store
        </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink is-active>Beranda</NavbarLink>
          <NavbarLink>Menu</NavbarLink>
          <NavbarLink>Tentang</NavbarLink>
        </NavbarCollapse>
      </template>
      <template #right-side>
        <button type="button" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Kontak</button>
      </template>
    </Navbar>
</template>
