<template>
  <view class="bottom-nav">
    <view class="bottom-nav-item">
      <uni-icons type="home" size="30"></uni-icons>
      <text>{{ state.textCN.home }}</text>
    </view>
    <view class="bottom-nav-item">
      <uni-icons type="more" size="30"></uni-icons>
      <text>{{ state.textCN.content }}</text>
    </view>
    <view class="bottom-nav-item">
      <uni-icons type="person" size="30"></uni-icons>
      <text>{{ state.textCN.me }}</text>
    </view>
  </view>
</template>

<script setup>
import { ref, reactive } from "vue";
import Content from '../Content/index.vue'
import Home from '../Home/index.vue'
import Me from '../Me/index.vue'

const state = reactive({
  textCN: {
    home: "Home",
    content: "Content",
    me: "Me",
  },
});
</script>

<style lang="scss">
.bottom-nav {
  width: 100%;
  height: 80px;
  display: flex;
  flex-flow: row nowrap;
  padding: 0;
  position: absolute;
  bottom: 0;

  &-item {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 14px;
    flex-direction: column;
  }
}
</style>
