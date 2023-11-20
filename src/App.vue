<template>

  <Layout />
  <Container />
 <!--  <ViewportInfo />   -->

 <ColumnFlex />

</template>
  

<script>
import Layout from './components/Layout.vue';
import Container from './components/Container.vue';
import ViewportInfo from './components/ViewportInfo.vue';
import ColumnFlex from './components/ColumnFlex.vue';


export default {
  name: 'App',
  components: { Layout, Container, ViewportInfo, ColumnFlex },

  setup() {


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
