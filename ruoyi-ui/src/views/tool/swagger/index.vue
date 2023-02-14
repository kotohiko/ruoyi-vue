<template>
  <i-frame :src="url" />
</template>
<script>
import iFrame from "@/components/iFrame/index";

export default {
  name: "Swagger",
  components: { iFrame },
  data() {
    return {
      // 属性名应该是url，而非src
      url: process.env.VUE_APP_BASE_API + "/doc.html"
    };
  },
};
</script>
