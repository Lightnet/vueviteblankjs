<script>

</script>
<template>
  <div>
    <router-link to="/">Home</router-link><span> | </span>
    <router-link to="/about">About</router-link><span> | </span>
    <router-link to="/errorpage">error page</router-link><span> | </span>
    <router-view v-slot="{ Component }">
      <Suspense>
        <component :is="Component" />
      </Suspense>
    </router-view>
  </div>
</template>

<style>

</style>