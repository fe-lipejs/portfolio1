<template>
  <div class="not-found">
    <h1>404 - Página não encontrada</h1>
    <p>A página que você está procurando não existe.</p>
  </div>
</template>

<script>
export default {
  name: 'NotFound'
}
</script>

<style scoped>
.not-found {
  text-align: center;
  margin-top: 50px;
}

h1 {
  font-size: 2em;
  color: #333;
}

p {
  font-size: 1.2em;
  color: #666;
}
</style>
