<script>
import ChuckJokes from './components/ChuckJokes.vue';

export default {
  components: {
    ChuckJokes,
  },
  data() {
    return {
      chuckJokes: [
        { value: "Chuck Norris can skydive into outer space."  },
        { value: "The chief export of Chuck Norris is pain."  },
        { value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { value: "Time waits for no man. Unless that man is Chuck Norris." },
        { value: "If you spell Chuck Norris in Scrabble, you win. Forever." },
        
      ],
    };
  },
};
</script>


<template>
  <div id="app">
    <ChuckJokes :chuckJokes="chuckJokes" />
  </div>
</template>
