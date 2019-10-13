<template>
  <div class="example">
    <h1>This is an Example page</h1>
    <h3>{{ message }}</h3>
  </div>
</template>

<script>
export default{
  name: "example",
  data(){
    return {
      message: "First Vue page"
    }
  }
}
</script>

<style scoped>
  h1 {
    color: red;
  }
</style>
