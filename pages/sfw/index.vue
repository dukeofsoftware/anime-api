<template>
  <div>
    <SelectComponent routeParam="sfw" :animeList="selects"></SelectComponent>
  </div>
</template>
<script>
export default {
  data() {
    return {
      selects: [
        "waifu",
        "neko",
        "shinobu",
        "megumin",
        "bully",
        "cuddle",
        "cry",
        "hug",
        "awoo",
        "kiss",
        "lick",
        "pat",
        "smug",
        "bonk",
        "yeet",
        "blush",
        "smile",
        "wave",
        "highfive",
        "handhold",
        "nom",
        "bite",
        "glomp",
        "slap",
        "kill",
        "kick",
        "happy",
        "wink",
        "poke",
        "dance",
        "cringe",
      ],
    };
  },
};
</script>
<style lang=""></style>
