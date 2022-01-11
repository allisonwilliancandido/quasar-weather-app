<template>
  <q-page class="flex flex-center">
    <q-card
      class="my-card"
      style="width: 300px; height: auto; display: flex; flex-direction: column; align-items: center"
    >
      <q-card-section>
        <q-img
          src="../assets/logo.png"
          ration="1"
          width="200px"
        />
      </q-card-section>

      <q-card-section class="q-pt-none full-width">
        <q-input
          v-model="email"
          filled
          type="email"
          label="E-mail"
        />

        <q-input
          v-model="login.password"
          filled
          :type="login.isPwd ? 'password' : 'text'"
          hint="Password with toggle"
        >
          <template v-slot:append>
            <q-icon
              :name="isPwd ? 'visibility_off' : 'visibility'"
              class="cursor-pointer"
              @click="login.isPwd = !isPwd"
              label="Password"
            />
          </template>
        </q-input>
      </q-card-section>
    </q-card>
  </q-page>
</template>

<script>
export default ({
  name: 'PageIndex',
  data () {
    return {
      login: {
        email: '',
        password: '',
        isPws: false
      }
    }
  },
  methods: {

  }
})
</script>
