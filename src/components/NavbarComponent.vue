<template>
  <q-header class="header bg-secondary row" elevated>
    <q-toolbar class="toolbar justify-around">
      <div class="row">
        <q-img class="logo-navbar" src="../assets/navbar-logo.png"></q-img>
        <div class="labels row items-center q-pl-lg q-pt-sm gt-xs">
          <h6>Label <q-icon name="arrow_drop_down" /></h6>
          <h6>Label <q-icon name="arrow_drop_down" /></h6>
          <h6>Label <q-icon name="arrow_drop_down" /></h6>
          <h6>Label <q-icon name="arrow_drop_down" /></h6>
        </div>
      </div>
      <q-btn class="gt-xs" no-caps unelevated rounded color="primary">
        <q-icon class="q-mr-sm" name="favorite" color="white" size="20px" />
        <div>Fazer doação</div>
      </q-btn>
      <!-- menu hamburguer -->
      <div class="xs">
        <q-btn flat dense round icon="menu" aria-label="Menu" />
      </div>
    </q-toolbar>
  </q-header>
</template>

<script setup>
//
</script>
