<!--App.vue-->
<script setup>
import PressScene from './view/PressScene.vue'
import MainScene from './view/MainScene.vue'
import { useSystemStore } from '@/store/system'
const store = useSystemStore()
</script>

<template>
  <PressScene v-if="store.scene == 'press'"></PressScene>
  <MainScene v-if="store.scene == 'play'"></MainScene>
</template>