<template>
  <div>
    <p class="font-bold text-gray-400 text-sm mb-1">Breadcrumbs</p>
    <h1 class="font-bold text-4xl">{{ name }}</h1>
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      default: "",
      required: false,
    },
  },
};
</script>

<style></style>
