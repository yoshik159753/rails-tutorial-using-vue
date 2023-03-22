<template>
  <header>
    <nav class="navbar navbar-expand navbar-dark bg-dark mb-4">
      <div class="container">
        <router-link :to="{ name: 'home' }" id="logo" class="navbar-brand">sample app</router-link>
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link :to="{ name: 'home' }" class="nav-link">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link :to="{ name: 'help' }" class="nav-link">Help</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/#" class="nav-link">Log in</router-link>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<style scoped lang="scss" >
#logo {
  float: left;
  margin-right: 10px;
  font-size: 1.7em;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: -1px;
  padding-top: 9px;
  font-weight: bold;

  &:hover {
    color: #fff;
    text-decoration: none;
  }
}
</style>
