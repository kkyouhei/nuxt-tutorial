<template>
  <ul>
    <li>hello</li>
    <router-link :to="{name: 'users-id', params: {id: userId}}" v-for="userId in [1,2,3,4,5]" :key="userId">
      <li>userId: {{ userId }}</li>
    </router-link>
  </ul>
</template>
<script>
export default {

}
</script>

