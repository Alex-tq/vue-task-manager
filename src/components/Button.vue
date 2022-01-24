<template>
  <button @click="onClick" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: {
      type: String,
    },
    color: {
      type: String,
      default: "black",
    },
  },
  methods: {
    onClick() {
      console.log("Button was clicked");
    },
  },
};
</script>
