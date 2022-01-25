<template>
  <div class="layout">
    <Header />

    <div class="content">
      <router-view v-slot="{ Component }">
        <transition name="fade" mode="out-in">
          <component :is="Component" />
        </transition>
      </router-view>
    </div>

    <Footer class=" end"/>
  </div>
</template>

<script>
import Header from "./components/header/Header.vue"
import Footer from "./components/footer/Footer.vue"

export default {
    componets: {
        Header
    },
    setup() {
    },
    components: { Header, Footer }
}
</script>

<style lang="scss" >

#app {
  font-family: "AvantGarde_bold", 'console';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--dark);
}

.layout {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 100%;
  margin: 0 auto;

}

</style>
