<script>
export default {
  name: 'ChuckCard',
  props: {
    iconUrl: String, // Define el prop 'iconUrl' como una cadena
    jokeValue: String, // Define el prop 'jokeValue' como una cadena
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


