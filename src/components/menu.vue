<template>
  <div v-show="showMenu" class="burger-menu">
    <ul>
      <li>Sample text</li>
      <li>Sample text</li>
      <li>Sample text</li>
      <li>Sample text</li>
      <li>Sample text</li>
    </ul>
  </div>
  <span v-on:click="toggleShowMenu()" class="material-icons flexCenter">notes</span>
</template>

<script>
export default {
  data() {
    return {
      showMenu: false
    }
  },
  methods: {
    toggleShowMenu() {
      this.showMenu = !this.showMenu
    }
  }
}
</script>

<style>
.material-icons {
  font-size: 40px;
  color: rgb(224, 221, 0);
  background-color: gray;
  border-radius: 3px;
  width: 45px;
  height: 45px;
  position: fixed;
  top: 20px;
  right: 20px;
  cursor: pointer;
}

ul {
  position: fixed;
  background-color: gray;
  right: 20px;
  top: 20px;
  list-style-type: none;
  border-radius: 3px;
  padding: 50px 20px;
}

li {
  color: rgb(224, 221, 0);
  font-weight: 600;
  font-size: 22px;
  margin: 10px;
  border-bottom: 2px solid gray;
  cursor: pointer;
}

li:hover {
  border-bottom: 2px solid white;
  transition: 500ms;
}

</style>