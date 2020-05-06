<template>
  <div class="main">
    <ul>
      <li v-for="todo in todos" :key="todo.time">
        {{ todo.text | capitalize }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Main",
  filters: {
    capitalize(val) {
      return val.toUpperCase();
    }
  },
  data() {
    return {
      todos: [
        { text: "Hello", time: 1524035 },
        { text: "sukthong", time: 2004035 }
      ]
    };
  }
};
</script>
