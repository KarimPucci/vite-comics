<script>
export default {
  name: "AppMain",
};
</script>

<template>
  <main>
    <nav class="entry">
      <a href="#">--> Content goes here --></a>
    </nav>
    <div class="jumbotron">
      <nav>
        <ul>
          <li><a href="#">DIGITAL COMICS</a></li>
          <li><a href="#">DC MERCHANDISE</a></li>
          <li><a href="#">SUBSCRIPTION</a></li>
          <li><a href="#">COMIC SHOP LOCATOR</a></li>
          <li><a href="#">DC POWER VISA</a></li>
        </ul>
      </nav>
    </div>
  </main>
</template>


<style lang='scss' scoped>
@use "../style/partials/mixin" as *;

main {
  width: 100%;
  height: 320px;
}

.entry {
  display: flex;
  justify-content: space-between;
  width: 100%;
  height: 120px;
  background-color: rgb(24, 23, 23);

  a {
    text-decoration: none;
    @include centerFlex("horizontal");
    padding-left: 200px;
    padding-top: 43px;
    font-weight: 600;
    font-size: 1.5rem;
    color: white;
  }
}

.jumbotron {
  justify-content: space-between;
  width: 100%;
  height: 130px;
  background-color: #0c7cec;

  ul {
    list-style: none;
    flex-direction: row;
    @include centerFlex("horizontal");
    padding-right: 600px;
    padding-top: 50px;
  }

  a {
    text-decoration: none;
    display: inline-block;
    padding: 10px;
    color: white;
    font-weight: 500;
  }
}
</style>