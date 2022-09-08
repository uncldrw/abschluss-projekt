<template>
  <table>
    <thead>
      <th>Klasse</th>
      <th>Anzahl der Schuler</th>
      <th>Person 3</th>
    </thead>
    <tr v-for="(entry, i) in 30" :key="i" @click="route">
      <td>BF420</td>
      <td>12</td>
      <td>21</td>
    </tr>
  </table>
</template>

<script>
export default {};
</script>

<style lang="scss">
table {
  @apply w-full;

  thead {
    @apply bg-gray-100;
  }
  td,
  th {
    @apply border-gray-200 py-1 px-2;
    &:not(:last-child) {
      @apply border-r;
    }
  }
  & > :not(:last-child) {
    @apply border-b border-gray-200;
  }
}
</style>
