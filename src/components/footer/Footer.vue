<template>
  <div class="footer">
    | <SocialLinks/> |
  </div>
</template>

<script>import { ref } from "vue"
import SocialLinks from "../nav/SocialLinks.vue"

export default {
    name: "footer",
    setup() {
        const year = ref(new Date().getFullYear());
        return {
            year
        };
    },
    components: { SocialLinks }
}
</script>

<style lang="scss">
  .footer {
    color: var(--primary);
    background-color: var(--dark);
    padding: 1em;
    display: flex;
    gap: 20px;
    justify-content: center;
  }

</style>