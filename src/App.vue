<script>
import ChuckJokes from './components/ChuckJokes.vue';
import ChuckCard from './components/ChuckCard.vue';

export default {
  components: {
    ChuckJokes,
    ChuckCard,
  },
  data() {
    return {
      chuckJokes: [
        { icon_url: "https://images.pexels.com/photos/12703416/pexels-photo-12703416.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
          value: "Chuck Norris can skydive into outer space."  },
        { icon_url: "https://images.pexels.com/photos/11833386/pexels-photo-11833386.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
          value: "The chief export of Chuck Norris is pain."  },
        { icon_url: "https://th.bing.com/th/id/OIP.xQO-5U7KSwU1neVaX00HHAHaE0?rs=1&pid=ImgDetMain",
          value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { icon_url: "https://th.bing.com/th/id/OIP.wVOujSiT5EqOWW0Bk_4ZPAHaE8?rs=1&pid=ImgDetMain",
          value: "Time waits for no man. Unless that man is Chuck Norris." },
        { icon_url: "https://th.bing.com/th/id/R.9922c49c8d8e29fa51f9b74f4456c766?rik=1DvdQYLhu4OS9A&riu=http%3a%2f%2fupload.wikimedia.org%2fwikipedia%2fcommons%2fc%2fcf%2fCurious_Raccoon.jpg&ehk=BexeDr3TN7SFeTzAur3PaOOACXatw1wJRTHY%2bMOJy5E%3d&risl=1&pid=ImgRaw&r=0",
          value: "If you spell Chuck Norris in Scrabble, you win. Forever." },
      ],
    };
  },
};
</script>


<template>
  <div>
    <h1>These are Chuck Jokes</h1>
  </div>
  <div id="app">
    <ChuckCard :iconUrl="chuckJokes[0].icon_url" :jokeValue="chuckJokes[0].value" />
    <ChuckCard :iconUrl="chuckJokes[1].icon_url" :jokeValue="chuckJokes[1].value" />
    <ChuckCard :iconUrl="chuckJokes[2].icon_url" :jokeValue="chuckJokes[2].value" />
    <ChuckCard :iconUrl="chuckJokes[3].icon_url" :jokeValue="chuckJokes[3].value" />
    <ChuckCard :iconUrl="chuckJokes[4].icon_url" :jokeValue="chuckJokes[4].value" />
  </div>
</template>
