<template>
  <h1>{{ name }}</h1>
  <p v-if="status === 'active'"> User is active </p>
  <p v-else>User is inactive</p>
  <h3>Tasks:</h3>
  <ul>
    <li v-for="task in tasks" :key="task">{{ task }}</li>
  </ul>
  <a v-bind:href="link">Click for Google</a> <!-- add any vue data to attribute use bind -->
  <a :href="link">Click for Google</a> <!-- shorter way to use v bind -->
</template>

<script>
export default{
  data(){
    return{
      name: 'John Doe',
      status:'active',
      tasks:[
        'Task 1',
        'Task 2',
        'Task 3',
      ],
      link: "https://google.com",
    };
  }
}
</script>
