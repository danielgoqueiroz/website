<template>
  <b-container fluid="sm">
    <b-form>
      <b-form-group default label="Envie um mensagem." label-for="input-1">
        <b-form-input
          v-model="form.nome"
          default
          type="text"
          placeholder="Nome"
          required
        />
        <b-form-input
          id="input-email"
          v-model="form.email"
          default
          type="email"
          placeholder="E-mail"
          required
        />
        <b-form-textarea
          id="textarea"
          v-model="form.text"
          default
          placeholder="Me escreva algo :)"
          rows="3"
          max-rows="6"
        />
      </b-form-group>
    </b-form>
  </b-container>
</template>

<script>
export default {
  name: 'Folio',
  data() {
    return {
      form: {
        name: '',
        email: '',
        text: '',
      },
    }
  },
  methods: {},
}
</script>

<style></style>
