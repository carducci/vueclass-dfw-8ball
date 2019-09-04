<template>
    <div class="answer-slot">
        {{chooseRandomAnswer()}}
    </div>
</template>

<script>
  import responses from '@/assets/responses.json';
    console.log(responses.responses);
  export default {

    name: "TheAnswer",
    methods: {
      chooseRandomAnswer: function() {
        return responses.responses[Math.floor(Math.random()*(responses.responses.length - 1))];
      }
    }
    // data: function() {
    //   return {
    //     responses
    //   }
    // }
  };
</script>

<style scoped>

</style>