<template lang="pug">
  .app
    h1 Привет, это портфолио на Vue + Pug + Stylus!
    p Скоро здесь будет больше проектов.
    button(@click="count++") Кликов: {{ count }}
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<style lang="stylus">
.app
  font-family Arial, sans-serif
  max-width 800px
  margin 0 auto
  padding 2rem
  text-align center

h1
  color red

button
  padding 0.5rem 1rem
  border none
  border-radius 4px
  background #42b883
  color white
  cursor pointer

  &:hover
    background #369e6f
</style>