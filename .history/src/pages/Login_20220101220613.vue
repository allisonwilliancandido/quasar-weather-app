<template>
  <q-page class="flex flex-center">
    <q-card
      class="my-card"
      style="width: 300px; height: auto; display: flex; flex-direction: column; ju"
    >
      <img
        src="../assets/logo.png"
        ration="1"
        width="200px"
      />

      <q-card-section>
        <div class="text-h5">Login</div>
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
