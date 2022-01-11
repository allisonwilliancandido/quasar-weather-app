<template>
  <q-page class="flex flex-center bg-primary">
    <q-card
      class="my-card"
      style="width: 500px; height: auto; display: flex; flex-direction: column; align-items: center"
    >
      <q-card-section>
        <q-img
          src="../assets/logo.png"
          ration="1"
          width="200px"
        />
      </q-card-section>

      <q-card-section class="q-gutter-md q-pt-none full-width">
        <q-input
          v-model="login.email"
          filled
          type="email"
          label="E-mail"
        />

        <q-input
          v-model="login.password"
          filled
          :type="login.isPwd ? 'password' : 'text'"
        >
          <template v-slot:append>
            <q-icon
              :name="login.isPwd ? 'visibility_off' : 'visibility'"
              class="cursor-pointer"
              @click="login.isPwd = !login.isPwd"
              label="Password"
            />
          </template>
        </q-input>
      </q-card-section>
      <q-card-actions>
        <q-btn
          size="lg"
          padding="10px lg 10px lg"
          color="primary"
          label="Login"
        />
      </q-card-actions>
      <q-card-actions>
        <q-btn
          no-caps
          flat
          size="lg"
          color="primary"
          label="Esqueci a senha"
          @click="$router.push({name: 'esquecisenha'})"
        />
      </q-card-actions>
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
        isPws: true
      }
    }
  },
  methods: {

  }
})
</script>
