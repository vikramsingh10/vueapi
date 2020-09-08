<template>
  <div id="app">
    <upper />
  
  </div>
</template>

<script>
 import upper from './components/upper';

 export default {
   name: 'app',
   components: {
     upper
   }

 }
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}

.btn {
  display: inline-block;
  border: none;
  background: grey;
  color: white;
  padding: 7px 20px;
  cursor: pointer;
}
</style>
