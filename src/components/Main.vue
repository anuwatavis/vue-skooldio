<template>
  <div class="main">{{ text + "Anuwat" }} {{ number + 10 }}</div>
</template>

<script>
export default {
  name: "Main",
  data() {
    return {
      text: "Hello World",
      number: 3
    };
  }
};
</script>
