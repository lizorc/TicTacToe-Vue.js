<template>
  <div @click="$emit('click')" class="cell">
    <span v-if="value !== ''" :class="{ 'pink' : value === 'x', 'blue': value === 'o' }">
      {{ value }}
    </span>
  </div>
</template>

<script>
  export default {
    props: {
      value: String,
    },
  }
</script>