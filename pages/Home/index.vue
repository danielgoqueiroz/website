<template>
  <div>
    <b-img :src="image.link" :alt="image.alt" fluid></b-img>
    <SobreCard />
    <InstagramPosts />
    <Folio />
    <ContatoForm />
  </div>
</template>

<script>
import SobreCard from '~/components/SobreCard'
import InstagramPosts from '~/components/InstagramPosts'
import Folio from '~/components/Folio'
import ContatoForm from '~/components/ContatoForm'

export default {
  name: 'Sobre',
  components: {
    SobreCard,
    InstagramPosts,
    Folio,
    ContatoForm,
  },
  data() {
    return {
      image: {
        alt: 'Imagem',
        link: require('~/assets/images/image.jpg'),
      },
    }
  },
}
</script>
<style></style>
