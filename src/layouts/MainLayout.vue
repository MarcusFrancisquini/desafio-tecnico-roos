<template>
  <q-layout view="lHh Lpr lFf">
    <!--? navbar -->
    <NavbarComponent />
    <!-- conteúdo da página -->
    <q-page-container>
      <router-view />
    </q-page-container>
    <!--? footer -->
    <FooterComponent />
  </q-layout>
</template>

<script setup>
import NavbarComponent from 'src/components/NavbarComponent.vue'
import FooterComponent from 'src/components/FooterComponent.vue'
</script>
