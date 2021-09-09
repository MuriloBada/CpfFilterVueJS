<template>
  <div class="CPF-Filter">
    <slot>{{ CPF | CpfFilter }}</slot>
  </div>
</template>

<script>
export default {
  filters: {
    CpfFilter(value) {
      const array = value.split("");
      array.splice(3, 0, ".");
      array.splice(7, 0, ".");
      array.splice(11, 0, "-");
      return array.join("");
    },
  },
  props: { CPF: { type: String, required: true } },
};
</script>

<style>
</style>