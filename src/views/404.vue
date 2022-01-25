<template>
    <Section class="notfound" >
      <img src="@/assets/img/404.svg" alt="not found image">
    </Section>
</template>

<script>
import Section from "../components/section/Section.vue";
export default {
    name: "404",
    components: { Section }
}

</script>

<style lang="scss" scoped>
.notfound {
  margin-top: 72px;
  height: calc(100vh - 72px - 52px);
}

img {
  width: min(80%, 450px);
}
</style>