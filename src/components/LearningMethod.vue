<template>
  <h1>Learning Method</h1>
  <p>{{ name }}</p>
  <p>Age: {{ age }}</p>
  <button @click="handleClick">Change</button>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    let name = ref("Nguyen Tuan Anh");
    let age = ref(20);

    function handleClick() {
      console.log("run");
    }

    setTimeout(() => {
      name.value = "Nguyen Tuan Anh 2";
      age.value = 21;
    }, 2000);
    return {
      name,
      age,
      handleClick,
    };
  },
};
</script>
