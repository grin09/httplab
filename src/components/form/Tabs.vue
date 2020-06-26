<template>
  <div class="tabs">
    <TabItem value="standard" :checked="tabselected" iconName="standard" caption="Standard" />
    <TabItem value="calendar" :checked="tabselected" iconName="calendar" caption="Event" />
    <TabItem value="alert" :checked="tabselected" iconName="alert" caption="Alert" />
  </div>
</template>

<script>
const TabItem = () => import("@/components/form/TabItem");
export default {
  components: {
    TabItem
  },
  data: function() {
    return {
      tabselected: "standard"
    };
  }
};
</script>

<style lang="scss" scoped>
.tabs {
  display: flex;
  justify-items: flex-start;
  align-items: center;
}
</style>