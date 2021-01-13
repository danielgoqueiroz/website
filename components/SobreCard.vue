<template>
  <div>
    <b-img :src="sobre.image" rounded="circle" alt="Circle image"></b-img>
    <h1>Daniel G. Queiroz</h1>
    <p>
      Sou publicitário de primeira formação, fotógrafo e videomaker por destino
      e desenvolvedor por determinação e paixão. Atuei por oito anos em jornal
      impresso diário. Em 2020 me formei em Análise e Desenvolvimento de
      Sistemas, área na qual sou apaixonado e na qual tenho feitos projetos
      pessoais. Após entrar como estagiário na Dígito Tecnologia, iniciei como
      deve júnior em Java.
    </p>
    <b-icon icon="instagram"></b-icon>
    <b-icon icon="facebook"></b-icon>
    <b-icon icon="linkedin"></b-icon>
    <b-icon icon="linkedin"></b-icon>
    <b-icon icon="github"></b-icon>
  </div>
</template>

<script>
export default {
  name: 'SobreCard',
  data() {
    return {
      sobre: {
        image: require('~/assets/images/sobre/danielgoqueiroz.jpg'),
      },
    }
  },
}
</script>

<style></style>
