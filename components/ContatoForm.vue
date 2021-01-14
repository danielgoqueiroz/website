<template>
  <b-container fluid>
    <h1>Contato</h1>
    <b-form>
      <b-form-group
        id="input-group-1"
        label="Endereço de e-mail:"
        label-for="input-1"
        description="Descrição"
      >
        <b-form-input
          id="input-1"
          v-model="form.email"
          type="email"
          placeholder="E-mail"
          required
        ></b-form-input>
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
        email: 'teste@email.com',
      },
    }
  },
  methods: {},
}
</script>

<style></style>
