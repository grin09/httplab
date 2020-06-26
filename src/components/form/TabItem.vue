<template>
  <label :class="['tab-item', {active: value == checked}]">
    <input :name="value" type="radio" :disabled="value == 'alert'" />
    <Icon :iconName="iconName" :iconColor="value == checked ? '#fff' : '#77838f'" />
    <span>{{ caption }}</span>
  </label>
</template>

<script>
const Icon = () => import("@/components/Icon");
export default {
  components: {
    Icon
  },
  props: {
    iconName: String,
    caption: String,
    value: String,
    checked: String
  }
};
</script>

<style lang="scss" scoped>
.tab-item {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  max-width: 150px;
  height: 40px;
  background-color: #e7eaf3;
  margin: 0 2px 0 0;
  &:first-child {
    border-radius: 24px 0 0 24px;
  }
  &:last-child {
    border-radius: 0 24px 24px 0;
    margin: 0;
  }
  &:disabled {
    filter: grayscale(1);
  }
  &.active {
    background-color: #377dff;
    span {
      color: #fff;
    }
  }
  input {
    display: none;
  }
  span {
    font-size: 16px;
    font-weight: 600;
    font-stretch: normal;
    font-style: normal;
    line-height: normal;
    letter-spacing: -0.07px;
    color: #77838f;
    margin: 0 0 0 8px;
  }
}
</style>