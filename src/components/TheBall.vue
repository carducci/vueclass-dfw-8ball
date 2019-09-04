<template>
    <div class="ball black">
        <TheAnswer>

        </TheAnswer>
        <TheCover>
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
    }
  }
</script>

<style>

</style>
