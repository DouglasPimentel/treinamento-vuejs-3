<template>
  <div>
    <h1 :style="{ textDecoration: decoration }">Hello {{ name }}</h1>
    <input type="text" v-model="name" />
    <br />
    <a :href="link">Link para site do Vue.js</a>
  </div>
</template>

<script>
export default {
  data: () => ({
    name: 'Vue.js Brasil',
    link: 'https://vuejs.org/',
    decoration: 'underline'
  })
}
</script>