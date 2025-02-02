<template>
  <q-layout view="lHh Lpr lFf">
    <!--? navbar -->
    <NavbarComponent />
    <!-- conteúdo da página -->
    <q-page-container>
      <router-view />
    </q-page-container>
    <!-- TODO colocar o Footer aqui também -->
  </q-layout>
</template>

<script setup>
import NavbarComponent from 'src/components/NavbarComponent.vue'
</script>
