<template>
  <Menu />
  <h1 class="flexCenter">Burger<br>Menu!</h1>
</template>

<script>
  import Menu from './components/Menu.vue'

export default { 
  components: {
    Menu
  }
}
</script>

<style>
  * {
    padding: 0;
    margin: 0;
    font-family: 'Courier New', Courier, monospace;
  }

  body {
    background-color: rgb(211, 211, 211);
  }
  
  .flexCenter {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  h1 {
    font-size: 100px;
    text-align: center;
    margin-top: 50px;
    color: rgb(75, 75, 75);
  }
</style>