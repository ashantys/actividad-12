<template>
    <div class="chuck-jokes">
    <ul>
        <li v-for="(joke, index) in chuckJokes" :key="index">{{ joke.value }}</li>
    </ul>
    </div>
</template>

<script>
export default {
    name: 'ChuckJokes',
    props: {
      chuckJokes: Array, 
    },
};
</script>

<style scoped>
.chuck-jokes {
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  padding: 10px;
  margin: 20px 0;
  border-radius: 5px;
}

.chuck-jokes ul {
  list-style: inside;
  padding: 0;
}

.chuck-jokes li {
  margin-bottom: 10px;
  font-size: 16px;
  color: #333;
}
</style>
