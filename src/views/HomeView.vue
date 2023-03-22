<template>
  <div class="center p-5 mb-4 bg-light rounded-3">
    <h1>Welcome to the Sample App</h1>

    <h2>
      This is the home page for the
      <a href="https://railstutorial.jp/">Ruby on Rails Tutorial</a>
      sample application.
    </h2>

    <router-link :to="{ name: 'Signup' }" class="btn btn-lg btn-primary">Sign up now!</router-link>
  </div>

  <a href="https://railstutorial.jp/"><img alt="Rails logo" src="../assets/rails.png" /></a>
</template>
