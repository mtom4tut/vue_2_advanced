<template>
  <router-link class="link" :to="href"> <slot /> </router-link>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'BaseLink',

  props: {
    href: {
      type: String,
      required: true,
    },
  },
})
</script>

<style lang="scss" scoped>
.link {
  transition: color 0.2s;

  &:hover {
  }
}
</style>
