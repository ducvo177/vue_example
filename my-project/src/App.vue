<template>
  <div>
    <button @click="unmountComponent">Unmount Component</button>
    <my-component v-if="mounted"></my-component>
  </div>
</template>

<script>
import MyComponent from './components/MyComponent.vue';

export default {
  components: {
    MyComponent,
  },
  data() {
    return {
      mounted: true,
    };
  },
  methods: {
    unmountComponent() {
      this.mounted = false;
    },
  },

};
</script>