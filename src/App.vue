<template>
  <div id="app">
    <h1>Liste des employés</h1>
    <EmployeeList />
  </div>
</template>

<script>
import EmployeeList from './components/EmployeeList.vue';

export default {
  name: 'App',
  components: {
    EmployeeList
  }
};
</script>

<style>
body {
  background-color: #20C997;
}
#app {
  display: flex;
  align-content: center;
  justify-content: center; 
  flex-direction: column;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
