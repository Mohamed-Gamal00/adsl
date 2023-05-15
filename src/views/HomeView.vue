<template>
  <div>
    <SecretImage />
  </div>
</template>

<script>
import { defineAsyncComponent } from "vue";
const SecretImage = defineAsyncComponent({
  loader: () => import("@/components/home/HomeCom.vue"),
});
export default {
  name: "HomeView",
  components: {
    SecretImage,
  },
};
</script>
