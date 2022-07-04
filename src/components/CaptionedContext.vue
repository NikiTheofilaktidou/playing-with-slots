
<template>
    <slot name="content">
        <img src="https://pbs.twimg.com/profile_images/3358404089/c5428a6dfa259ff80f23ea4b9abb050b_400x400.jpeg" alt="">
    </slot>
    <br>
    <slot name="caption" v-bind:source="source">Caption</slot>
</template>

<script>

export default {
  data(){
    return {
      source: 'YouTube',
    }
  }
}
</script>

<style scoped>
img {
    width:100%;
}
</style>
