<template>
  <q-page class="flex flex-center">
    <q-card
      class="my-card"
      style="width: 300px; height: auto; display: flex; flex-direction: column; align-items: center"
    >
    <q-card-section></q-card-section>      

      <q-card-section>
        <div class="text-h5">Login</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        <q-input filled v-model="text" label="Filled" />
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
