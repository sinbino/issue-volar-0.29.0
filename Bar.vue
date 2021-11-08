<!--
This template will cause the following error in volar v0.29.0

  Extraneous children found when component already has explicitly named default slot. These children will be ignored.
  ```html
  <x__VLS_ />
  ```vue(39)
  (property) template: any
  The template element is used to declare fragments of HTML that can be cloned and inserted in the document by script.
-->

<template lang="pug">
Foo
  template(v-slot:header)
    div FOO

  template(v-slot)
    div Bar
</template>

<script>
import Foo from './Foo.vue'

export default {
  components: {Foo},
}
</script>
