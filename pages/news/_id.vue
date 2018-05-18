<template>
  <div>
    <h2>newscontent[{{$route.params.id}}]</h2>
    <ul>
      <li><a href="/">Home</a></li>
    </ul>
  </div>
</template>

<script>
  export default {
    validate ({ params }) {
      // Must be a number
      return /^\d+$/.test(params.id)
    }
  }
</script>

<style scoped>

</style>
