<script>
export default {
  mounted() {
    $fetch("http://google.com/404").then((ctx) => {
      console.log(ctx);
    });
  },
  computed: {
    hideHeader() {},
  },
};
</script>

<template>
  <Navigation />
  <NuxtPage class="pl-72 pr-12 pt-10" />
</template>
