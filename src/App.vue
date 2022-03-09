<template>
<n-space>
I'm trying to set the most restrictive <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP">CSP</a> possible, however as an example, the buttons below have inline styles that then require 'unsafe-inline' style-src.
</n-space>
   <n-space>
    <n-button>Default</n-button>
    <n-button type="tertiary">
      Tertiary
    </n-button>
    <n-button type="primary">
      Primary
    </n-button>
    <n-button type="info">
      Info
    </n-button>
    <n-button type="success">
      Success
    </n-button>
    <n-button type="warning">
      Warning
    </n-button>
    <n-button type="error">
      Error
    </n-button>
  </n-space>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { NSpace, NButton } from 'naive-ui';

export default defineComponent({
  name: 'App',
  components: {
    NSpace,
    NButton
  }
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
