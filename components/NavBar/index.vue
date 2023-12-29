<template>
  <ul>
    <li 
    v-for="item in navItems"
    :key="item"
    >
      <a :href="item.link">
        <NavItem :item="item" />
      </a>
    </li>
  </ul>
</template>

<script setup>
import NavItem from './components/NavItem.vue'

const navItems = [
  {
    name: "Home",
    link: "/"
  },
  {
    name: "menu",
    link: "/menu"
  },
	{
   name: "galeria",
   link: "/gallery"
	},
  {
   name: "kontakt",
   link: "/contact"
	}
];
</script>