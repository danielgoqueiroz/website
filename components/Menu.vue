<template>
  <div>
    <b-navbar>
      <b-navbar-brand><Logo class="logo" /></b-navbar-brand>
      <b-navbar-nav class="ml-auto">
        <NuxtLink
          v-for="item in menu"
          :key="item.title"
          class="menu-item"
          :to="item.link"
          >{{ item.title }}
        </NuxtLink>
      </b-navbar-nav>
    </b-navbar>
  </div>
</template>

<script>
import Logo from '~/components/Logo'
export default {
  name: 'Menu',
  components: {
    Logo,
  },
  data() {
    return {
      logo: {
        title: 'Home',
        link: '/home',
      },
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
nav .logo {
  float: left;
  margin-left: 15px;
  margin-right: 15px;
  text-align: center;
  border-bottom: 3px solid transparent;
  transition: 0.3s;
}
nav {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgb(49, 49, 49);
}

nav .menu-item {
  color: aliceblue;
  padding: 10px 30px;
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
