<!--
This template will cause the following error in volar v0.29.0

  v-else/v-else-if has no adjacent v-if or v-else-if.vue(30)
  (property) x__VLS_: any
-->

<template lang="pug">
div
  slot(name="header")

  div.foo(v-if="cond")
    slot

  div.bar(v-else)
    slot
</template>

<script>
export default {
  data() {
    return {
      cond: true,
    }
  },
}
</script>
