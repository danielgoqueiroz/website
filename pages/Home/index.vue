<template>
  <div>
    <b-img :src="image.link" :alt="image.alt" fluid></b-img>
    <SobreCard />
    <InstagramPosts />
    <h1>últimos trabalhos</h1>
    <h1>contato</h1>
  </div>
</template>

<script>
import SobreCard from '~/components/SobreCard'
import InstagramPosts from '~/components/InstagramPosts'

export default {
  name: 'Sobre',
  components: {
    SobreCard,
    InstagramPosts,
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
