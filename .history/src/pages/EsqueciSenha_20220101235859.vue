<template>
  <q-page class="flex flex-center bg-primary">
    <q-card
      class="my-card"
      style="width: 500px; height: auto; display: flex; flex-direction: column; align-items: center"
    >
      <q-card-section class="full">
        <p class="text-h5">Esqueci minha senha</p>
        <p class="text-caption">Informe o e-mail para recuperar a senha</p>

      </q-card-section>
      <q-card-section class="q-gutter-md q-pt-none full-width">
        <q-input
          v-model="login.email"
          filled
          type="email"
          label="Redefinir senha"
          pa
        />
      </q-card-section>
      <q-card-actions>
        <q-btn
          outline
          size="lg"
          padding="10px lg 10px lg"
          color="primary"
          label="Redefinir Senha"
          @click="$router.push({name: 'login'})"
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
