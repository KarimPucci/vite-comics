<script>
export default {
  name: "AppHeader",
};
</script>

<template>
  <header>
    <div class="logo">
      <img src="/dc-logo.png" alt="Logo DC" />
    </div>

    <nav>
      <ul>
        <li><a href="#">CHARACTERS</a></li>
        <li><a href="#" class="active">COMICS</a></li>
        <li><a href="#">MOVIES</a></li>
        <li><a href="#">TV</a></li>
        <li><a href="#">GAMES</a></li>
        <li><a href="#">COLLECTIBLES</a></li>
        <li><a href="#">VIDEO</a></li>
        <li><a href="#">FANS</a></li>
        <li><a href="#">NEWS</a></li>
        <li><a href="#">SHOP</a></li>
      </ul>
    </nav>
  </header>
</template>


<style lang="scss" scoped>
@use "../style/partials/mixin" as *;

header {
  display: flex;
  justify-content: space-between;
  width: 100%;
  height: 130px;
  background-color: green;
  .logo {
    padding-left: 200px;
    padding-top: 10px;
  }
  ul {
    list-style: none;
    flex-direction: row;
    @include centerFlex("horizontal");
    padding-right: 200px;
    padding-top: 50px;
    a {
      text-decoration: none;
      display: inline-block;
      padding: 10px;
      color: black;
      font-weight: 500;
      &:hover,
      &.active {
        background-color: lightblue;
      }
    }
  }
}
</style>