<template>
  <div>
    <button @click="back" class="nav-button"><span>&#8592;</span></button>
  </div>
</template>

<script>
import router from "@/index/router";

export default {
  methods: {
    back() {
      router.back();
    },
  },
};
</script>
