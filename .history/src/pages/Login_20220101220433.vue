<template>
  <q-page class="flex flex-center">
    <q-card class="my-card">
      <img src="../assets/logo.png">

      <q-card-section>
        <div class="text-h6">Login</div>
        <div class="text-subtitle2">by John Doe</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'PageIndex'
})
</script>
