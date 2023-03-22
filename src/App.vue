<template>
  <ApplicationLayout>
    <router-view />
  </ApplicationLayout>
</template>

<script>
import ApplicationLayout from './components/layouts/ApplicationLayout.vue';

export default {
  components: {
    ApplicationLayout
  },
  mounted() {
    this.setTitle(this.$route.meta.title);
  },
  watch: {
    '$route'(routeInstance) {
      this.setTitle(routeInstance.meta.title);
    }
  },
  methods: {
    setTitle(title) {
      /**
       * title の差し替えに関するテクニックは下記を参照。
       * ref. https://prograshi.com/language/vue-js/set-title-and-description-in-vue-cli-project/
       */
      if (title) {
        document.title = `${title} | Ruby on Rails Tutorial Sample App`;
      } else {
        document.title = 'Ruby on Rails Tutorial Sample App'
      }
    }
  }
}
</script>
