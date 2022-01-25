<template>
  <div :class="`featured-list ${type}`">
    <router-link to="#" class="featured-item"><i class=" icon-linkedin"></i></router-link>
    <router-link to="#" class="featured-item"><i class=" icon-facebook"></i></router-link>
    <router-link to="#" class="featured-item"><i class=" icon-twitter"></i></router-link>
    <router-link to="#" class="featured-item"><i class=" icon-instagram"></i></router-link>
  </div>
</template>

<script>
import { ref } from "vue"

export default {
  name: 'Nav',
  props: {
    type: {
      type: String,
      default: ''
    }
  },
  setup( ) {
    const isMenuVisible = ref(false)

    // Show/hide the menu panel
    const toogleMenu = () => {
      isMenuVisible.value = !isMenuVisible.value
    }

    return {
      isMenuVisible,
      toogleMenu
    }
  }
}
</script>

<style lang="scss">
.featured {

  &-list {
    display: flex;
    gap: 1em;


    &.dark > * {
      color: #222;
    }
  }

  &-item {
    font-size: 20px;
    color: #fff;
    text-decoration: none;

    & i {
      display: flex;
      place-items: center;
    }
  }
}

</style>