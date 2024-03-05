<template>
  <div>
    <header class="header container">
    <img class="header__logo" src="../assets/img/logo.png" alt="logo">
    <div class="header__links">
      <a class="header__link" href="#">Home</a>
      <a class="header__link" href="#">Project</a>
      <a class="header__link" href="#">Blog</a>
    </div>
  </header>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>
  * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

a {
  text-decoration: none;
  color: inherit;
}

ul {
  list-style: none;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

.header{
  margin-top: 44px;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 57px;
}

.header__logo{
  height: 50px;
}

.header__links {
  display: flex;
  text-align: center;
  gap: 50px;
  font-size: 20px;
  line-height: 25px;
  align-items: center;
  font-family: "Jost";
  font-weight: 400;
  color: #292F36;
}
</style>