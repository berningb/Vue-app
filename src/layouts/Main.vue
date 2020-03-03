<template>
  <div class="container-fluid">
    <ul>
      <li>
        <v-link href="/">Home</v-link>
        <v-link href="/about">About</v-link>
      </li>
    </ul>

    <slot></slot>
  </div>
</template>

<script>
  import VLink from '../components/VLink.vue'

  export default {
    components: {
      VLink
    }
  }
</script>

<style scoped>
  ul {
    background-color: white
  }
  .container-fluid {
    padding: 0px;
  }

  ul {
    list-style: none;

  }
  a:link {
    color: black;
  }

  a:visited {
    color: black;
  }

  a:hover {
    color: grey;
  }

  a:active {
    color: grey;
}
</style>
