<template>
    <div class="ball black" v-on:click="shake()">
        <TheAnswer v-if="shook">
        </TheAnswer>
        <TheCover v-if="!shook">
            8
        </TheCover>

    </div>
</template>

<script>
  import TheAnswer from '@/components/TheAnswer';
  import TheCover from '@/components/TheCover';
  export default {
    name: 'TheBall',
    components:{
      TheAnswer,
      TheCover
    },
    data: function() {
      return {
        shook: false
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
