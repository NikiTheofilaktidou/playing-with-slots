
<template>
  <captioned-context>
    <template #content>
    <img src="https://cdn.pixabay.com/photo/2015/03/10/17/26/facebook-667456__340.png"/>
    </template>
    <br/>
    <br/>
    <template v-slot:caption >
      Just a plain old fb logo
    </template>
  </captioned-context>
  <br/>
  <br/>
   <captioned-context>
    <template #content>
    <iframe 
    width="560" 
    height="315" 
    src="https://www.youtube.com/embed/X5oD_thIk3c" 
    title="YouTube video player" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen></iframe>
    </template>
    <template v-slot:caption="{ source }">
      Source: <a href="https://www.youtube.com">{{ source }}</a>
    </template>
  </captioned-context>
  <div>
    <br>
    <br>
    Slots worked c:
  </div>
</template>

<script>
import CaptionedContext from './components/CaptionedContext.vue'

export default {

  name: 'App',
  components: {
    CaptionedContext  
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
