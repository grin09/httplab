<template>
  <div class="home">
    <div class="container">
      <Form />
    </div>
  </div>
</template>

<script>
const Form = () => import("@/components/Form");
export default {
  components: {
    Form
  }
};
</script>

<style lang="scss" scoped>
.home {
  width: 100%;
  max-width: 512px;
  box-shadow: 0 8px 8px 0 rgba(119, 131, 143, 0.16);
}
.container {
  width: 100%;
  background-color: #fff;
}
</style>