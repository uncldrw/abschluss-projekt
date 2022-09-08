<template>
  <aside class="bg-gray-100 h-screen fixed w-60 px-6 flex flex-col">
    <div class="pt-16">
      <p class="font-bold text-4xl">ATIW</p>
    </div>
    <ul class="h-full">
      <li v-for="(item, i) in menu" :key="i">
        <NuxtLink :to="item.route">
          {{ item.name }}
        </NuxtLink>
      </li>
    </ul>
    <p class="pb-16">Logout</p>
  </aside>
</template>

<script>
export default {
  data: () => ({
    menu: {
      classes: {
        name: "Klassen",
        route: "/",
      },
      pupils: {
        name: "Schüler",
        route: "pupils",
      },
      businesses: {
        name: "Betriebe",
        route: "businesses",
      },
    },
  }),
};
</script>

<style></style>
