<template>
  <div id="app">
    <Header />
    <Top />
    <Profile />
    <Skills />
    <Works />
    <More />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import Top from './components/Top.vue'
import Profile from './components/Profile.vue'
import Skills from './components/Skills.vue'
import Works from './components/Works.vue'
import More from './components/More.vue'


export default {
  name: 'App',
  components: {
    Header,
    Top,
    Profile,
    Skills,
    Works,
    More
  },
}
</script>

<style>
h1{
  margin: 0;
}

body{
  font-family: 'Source Serif Pro', serif;
}

section{
  margin-bottom: 20px;
}

.section-title-wrapper{
  text-align: center;
  padding: 20px;
}
</style>