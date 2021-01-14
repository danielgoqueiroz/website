<template>
  <b-container fluid="sm">
    <b-row>
      <b-col>
        <h1>Contato</h1>
      </b-col>
    </b-row>
    <b-row>
      <b-col>
        <ContatoForm />
      </b-col>
    </b-row>
  </b-container>
</template>
<script>
import ContatoForm from '@/components/ContatoForm'
export default {
  components: {
    ContatoForm,
  },
}
</script>
<style></style>
