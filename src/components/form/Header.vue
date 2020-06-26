<template>
  <div class="form-header">
    <h1>{{ title }}</h1>
    <span>{{ description }}</span>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    description: String
  }
};
</script>

<style lang="scss" scoped>
.form-header {
  h1 {
    font-size: 24px;
    font-weight: bold;
    font-stretch: normal;
    font-style: normal;
    line-height: normal;
    letter-spacing: -0.11px;
    color: #000000;
    margin: 0 0 2px;
  }
  span {
    font-size: 18px;
    font-weight: 600;
    font-stretch: normal;
    font-style: normal;
    line-height: normal;
    letter-spacing: -0.08px;
    color: #828e9a;
  }
}
</style>