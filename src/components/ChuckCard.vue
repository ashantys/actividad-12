<script>
export default {
  name: 'ChuckCard',
  props: {
    iconUrl: String, 
    jokeValue: String, 
  },
};
</script>

<template>
    <div class="chuck-card">
    <div class="card">
        <img :src="iconUrl" class="card-img-top" alt="Chuck Norris">
        <div class="card-body">
        <p class="card-text">{{ jokeValue }}</p>
        </div>
    </div>
    </div>
</template>

<style scoped>
.chuck-card {
  max-width: 300px;
  margin: 10px;
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  padding: 10px;
  border-radius: 5px;
}

.card-img-top{
  border-radius: 5px;
  max-width: 250px;
}

.card-text {
  margin-bottom: 10px;
  font-size: 16px;
  color: #333;
}
</style>


