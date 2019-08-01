<template>
  <div>
    <div>hello show user {{userId}}</div>
    <n-link :to="{name: 'users-id-profile'}">
      link to profile
    </n-link>
    <nuxt-child></nuxt-child>
  </div>
</template>
<script>
export default {
  transition: 'bounce',
  computed: {
    userId () {
      return this.$route.params.id
    }
  },
}
</script>

