<template>
  <form>
    <Header title="Traffic Runners, LLC" description="Softwear company" />
    <Tabs />
  </form>
</template>

<script>
const Header = () => import("@/components/form/Header");
const Tabs = () => import("@/components/form/Tabs");
export default {
  components: {
    Header,
    Tabs
  }
};
</script>

<style lang="scss" scoped>
.tabs {
  margin: 26px 0 0;
}
</style>