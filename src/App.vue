<template>
  <div id="app">
    <List />
    <Footer/>
  </div>
</template>

<script>
import List from "./components/List";
import Footer from './components/Footer'

export default {
  name: "App",
  components: {
    List,
    Footer
  },
};
</script>

<style />
