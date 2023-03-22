<template>
  <footer class="footer">
    <small>
      The <a href="https://railstutorial.jp/">Ruby on Rails Tutorial</a>
      by <a href="http://www.michaelhartl.com/">Michael Hartl</a>
    </small>
    <nav>
      <ul>
        <li>
          <router-link :to="{ name: 'about' }">About</router-link>
        </li>
        <li>
          <router-link :to="{ name: 'contact' }">Contact</router-link>
        </li>
        <li><a href="http://news.railstutorial.org/">News</a></li>
      </ul>
    </nav>
  </footer>
</template>

<style scoped lang="scss">
@import '@/assets/variables.scss';

footer {
  margin-top: 45px;
  padding-top: 5px;
  border-top: 1px solid $gray-medium-light;
  color: $gray-light;

  a {
    color: $gray;

    &:hover {
      color: $gray-darker;
    }
  }

  small {
    float: left;
  }

  ul {
    float: right;
    list-style: none;

    li {
      float: left;
      margin-left: 15px;
    }
  }
}
</style>
