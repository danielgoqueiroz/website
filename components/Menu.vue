<template>
  <nav>
    https://www.youtube.com/watch?v=vUcUdpBcmF8
    <div v-for="item in menu" :key="item.title" class="menu-item">
      {{ item.title }}
      <a :href="item.link"></a>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Menu',
  data() {
    return {
      menu: [
        {
          title: 'Home',
          link: '/home',
        },
        {
          title: 'Sobre',
          link: '/sobre',
        },
        {
          title: 'Contato',
          link: '/contato',
        },
      ],
    }
  },
}
</script>

<style>
nav {
  display: flex;
  align-items: center;
  justify-content: center;
}

nav .menu-item {
  color: aliceblue;
  padding: 10px 20px;
  position: relative;
  text-align: center;
  border-bottom: 3px solid transparent;
  display: flex;
  transition: 0.3s;
}

nav .menu-item.active,
nav .menu-item:hover {
  background-color: rgb(44, 44, 44);
  border-bottom-color: rgb(255, 225, 0);
}
</style>
