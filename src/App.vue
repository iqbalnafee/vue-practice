<template>
  <h1>{{ name }}</h1>
  <p v-if="status === 'active'"> User is active </p>
  <p v-else>User is inactive</p>
</template>

<script>
export default{
  data(){
    return{
      name: 'John Doe',
      status:'active',
    };
  }
}
</script>
