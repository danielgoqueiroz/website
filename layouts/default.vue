<template>
  <div>
    <Menu />
    <Nuxt />
  </div>
</template>
<script>
import Menu from '~/components/Menu'
export default {
  components: {
    Menu,
  },
}
</script>
<style>
html {
  /* font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  margin: 0;
  height: 100%;
  width: 100%; */
}

*,
*::before,
*::after {
  margin: 0;
}
</style>
