<template>
  <q-header class="header bg-secondary row justify-center">
    <div class="row custom-spacing-border">
      <q-toolbar class="toolbar row items-center justify-between no-padding">
        <div class="row">
          <q-img class="logo-navbar" src="../assets/navbar-logo.png"></q-img>
          <div class="labels row items-center q-pl-lg q-pt-sm mobile-out">
            <h6>Label <q-icon name="arrow_drop_down" /></h6>
            <h6>Label <q-icon name="arrow_drop_down" /></h6>
            <h6>Label <q-icon name="arrow_drop_down" /></h6>
            <h6>Label <q-icon name="arrow_drop_down" /></h6>
          </div>
        </div>
        <q-btn class="mobile-out" no-caps unelevated rounded color="primary">
          <q-icon class="q-mr-sm" name="favorite" color="white" size="20px" />
          <div>Fazer doação</div>
        </q-btn>
        <!-- menu hamburguer -->
        <div class="menu-mobile">
          <q-btn flat dense round icon="menu" aria-label="Menu" />
        </div>
      </q-toolbar>
    </div>
  </q-header>
</template>

<script setup>
//
</script>
