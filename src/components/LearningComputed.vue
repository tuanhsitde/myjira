<template>
  <div><input type="text" placeholder="FirstName" @input="setFirstName" /></div>
  <div><input type="text" placeholder="Lastname" @input="setLastName" /></div>
  <div>
    <p>FirstName:</p>
    <p>LastName:</p>
    <p>Name : {{ fullName }}</p>
  </div>
</template>

<script>
import { computed, ref } from "vue";

export default {
  name: "LearningComputed",
  setup() {
    const firstName = ref("");
    const lastName = ref("");

    function setFirstName(event) {
      firstName.value = event.target.value;
    }

    function setLastName(event) {
      lastName.value = event.target.value;
    }

    const fullName = computed(() => firstName.value + lastName.value);
    return {
      setFirstName,
      setLastName,
      firstName,
      fullName,
    };
  },
};
</script>
<style>
template {
  display: block;
}
</style>
