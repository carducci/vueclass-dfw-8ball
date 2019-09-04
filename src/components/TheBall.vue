<template>
    <div class="ball black" v-on:click="shake()">
        <TheAnswer v-if="shook">
            answer
        </TheAnswer>
        <TheCover v-if="!shook">
            8
        </TheCover>

    </div>
</template>

<script>
  import TheAnswer from '@/components/TheAnswer';
  import TheCover from '@/components/TheCover';
  import responses from '@/assets/responses.json';
  export default {
    name: 'TheBall',
    components:{
      TheAnswer,
      TheCover
    },
    data: function() {
      return {
        shook: false,
        responses,
      }
    },
    methods: {
      shake: function() {
        this.shook = !this.shook;
      }
    }
  }
</script>

<style>

</style>
