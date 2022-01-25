<template>
  <div class="header-bg" :data-show="isScrollingUp">
    <div class="header">
      <router-link :to="{ path: '/', hash :'#welcome'}">
        <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 486.64 100.14" class="header-logo">
          <defs>
            <linearGradient id="Degradado_sin_nombre_2" y1="451.23" x2="107.11" y2="451.23"
              gradientTransform="matrix(1, 0, 0, -1, 0, 501.3)" gradientUnits="userSpaceOnUse">
              <stop offset="0" stop-color="#8ac9b4" />
              <stop offset="1" stop-color="#94cba4" />
            </linearGradient>
          </defs>
          <g id="Capa_1" data-name="Capa 1">
            <path class="cls-1"
              d="M43.21,17.37,45.64,3.89A5.17,5.17,0,0,1,51,0h50.41s6.3.48,5.68,5.82-3.87,20.51-3.87,20.51-2.1,4.37-4.69,4.52-83.21,0-83.21,0a.87.87,0,0,0-.65.12,1.37,1.37,0,0,0-.2.29c-1,1.81-1.79,3.61-1.16,4.3a1.27,1.27,0,0,0,.87.32H85.26a6,6,0,0,1,3.95,1.28,6.26,6.26,0,0,1,2.19,4.69Q90,50.59,88.65,59.31A8.09,8.09,0,0,1,85,64.43a5.76,5.76,0,0,1-1.34.53H37.39a2.24,2.24,0,0,0-.65.21,2.56,2.56,0,0,0-1.13,1.89q-.88,5.1-1.78,10.18A1.5,1.5,0,0,0,34,78.46a1.44,1.44,0,0,0,.68.56H46.12l1.94-7.92a1.22,1.22,0,0,1,1.57-.71,1.28,1.28,0,0,1,.37.23L67.13,82.57a1.12,1.12,0,0,1,.39.85,1,1,0,0,1-.55.93L43.86,99.86a1.35,1.35,0,0,1-1.66,0,1.45,1.45,0,0,1-.45-1.18c.71-2.47,1.4-5,2.11-7.42L25.92,91.1a5.39,5.39,0,0,1-2.13-.49c-3.23-1.51-3.65-5.77-3.68-6.14L25,58a5.7,5.7,0,0,1,.94-2.44,6.36,6.36,0,0,1,4.88-2.4L77.31,53a1.22,1.22,0,0,0,.36-.18,1.75,1.75,0,0,0,.65-.91l.6-3.59L5.41,47.83A5.91,5.91,0,0,1,1.2,45.61,6,6,0,0,1,.07,41.09L3.7,23.6a6.74,6.74,0,0,1,2.67-3.43A6.13,6.13,0,0,1,9,19.24l82.42-.17a1.62,1.62,0,0,0,.51-.21,3,3,0,0,0,1.27-2.05l.63-5a1.14,1.14,0,0,0-.39-.48,1.19,1.19,0,0,0-.58-.17L57.92,11a1.59,1.59,0,0,0-.73.37,1.78,1.78,0,0,0-.57.92c-.21,1.67-.42,3.34-.65,5Z" />
          </g>
          <g id="Capa_1-2" data-name="Capa 1-2">
            <path class="cls-2" d="M114.27,20.57h17.94v8h-9.9v6h9.54v7.94h-9.54V56h-8Z" />
            <path class="cls-2"
              d="M161.87,56H154.5V53.12h-.09c-1.24,2.58-4.31,3.78-7.19,3.78-7.82,0-12.39-6.6-12.39-14.21,0-8.71,5.82-14.17,12.39-14.17,4,0,6.31,2.1,7.19,3.73h.09V29.43h7.37Zm-13.54-6.51c4.62,0,6.17-4.21,6.17-6.79,0-3.21-2-6.75-6.22-6.75s-6.08,3.83-6.08,6.84C142.2,45.27,143.89,49.48,148.33,49.48Z" />
            <path class="cls-2"
              d="M177.28,36.89c0-.57-.13-2-2.31-2a1.87,1.87,0,0,0-2.09,1.78c0,1.43,1.83,2.24,3.78,2.87,4.17,1.24,8.62,2.58,8.62,8.33s-4.58,9-10,9c-3.73,0-9.37-1.82-10-8.81h7.33a2.65,2.65,0,0,0,2.8,2.45c1.24,0,2.57-.77,2.57-2.06,0-2.06-1.82-2.3-6.53-4.26-3.19-1.1-5.86-3.35-5.86-6.94,0-5.27,4.44-8.76,9.55-8.76,3.24,0,8.84,1.39,9.46,8.37Z" />
            <path class="cls-2" d="M197.35,29.43h3.55v6h-3.55V56H190V35.46h-3.64v-6H190V20.57h7.37Z" />
            <path class="cls-2" d="M221.2,28.52h-6.49V20.57H236v8h-6.44V56H221.2Z" />
            <path class="cls-2"
              d="M238.6,29.43h6.93v2.82h.09c.62-1.29,1.91-3.73,6.17-3.73v8c-3.42.1-5.82.86-5.82,4.88V56H238.6Z" />
            <path class="cls-2"
              d="M280.21,56h-7.37V53.12h-.09c-1.24,2.58-4.31,3.78-7.2,3.78-7.81,0-12.39-6.6-12.39-14.21,0-8.71,5.82-14.17,12.39-14.17,4.05,0,6.31,2.1,7.2,3.73h.09V29.43h7.37Zm-13.54-6.51c4.61,0,6.17-4.21,6.17-6.79,0-3.21-2-6.75-6.22-6.75s-6.08,3.83-6.08,6.84C260.54,45.27,262.22,49.48,266.67,49.48Z" />
            <path class="cls-2"
              d="M310.05,45.89c-1.33,6-6.26,11-12.92,11-7.46,0-13.19-6.31-13.19-14.21s5.64-14.12,13-14.12A13.3,13.3,0,0,1,310,39.67h-7.46a5.55,5.55,0,0,0-5.33-3.73c-3.51-.19-5.87,2.92-5.87,6.75s2.36,6.74,5.87,6.74a5.66,5.66,0,0,0,5.33-3.54Z" />
            <path class="cls-2"
              d="M313.91,20.57h7.37V39.05h.09l6.84-9.62H337l-9.28,11.68,9,14.88h-8.35l-7-12.78h-.09V56h-7.37Z" />
            <path class="cls-2" d="M357.87,28.52h-6.48V20.57H372.7v8h-6.44V56h-8.39Z" />
            <path class="cls-2"
              d="M401.21,56h-7.37V53.12h-.09c-1.24,2.58-4.31,3.78-7.19,3.78-7.82,0-12.39-6.6-12.39-14.21,0-8.71,5.81-14.17,12.39-14.17,4,0,6.3,2.1,7.19,3.73h.09V29.43h7.37Zm-13.54-6.51c4.62,0,6.17-4.21,6.17-6.79,0-3.21-2-6.75-6.22-6.75s-6.08,3.83-6.08,6.84C381.54,45.27,383.23,49.48,387.67,49.48Z" />
            <path class="cls-2" d="M406.14,20.57h7.37V56h-7.37Z" />
            <path class="cls-2"
              d="M442.15,47.66a15.4,15.4,0,0,1-5,6.8,11.37,11.37,0,0,1-7,2.39c-7.07,0-13.06-6.17-13.06-14.07,0-7.42,5.42-14.26,12.92-14.26s13,6.41,13,14.5a11.7,11.7,0,0,1-.18,2.11H424.34a5.65,5.65,0,0,0,5.78,5,5.14,5.14,0,0,0,4.48-2.49Zm-6.53-7.89a5.72,5.72,0,0,0-11.19,0Z" />
            <path class="cls-2"
              d="M446.63,29.43h6.89v2.82h.09c.75-1.29,2.3-3.73,6.7-3.73a10.1,10.1,0,0,1,6.31,2.3c1.33,1.24,2.84,3.35,2.84,8.56V56h-7.37V41.49c0-1.87,0-5.5-3.87-5.5C454,36,454,39.91,454,41.54V56h-7.37Z" />
            <path class="cls-2" d="M483.09,29.43h3.55v6h-3.55V56h-7.37V35.46h-3.64v-6h3.64V20.57h7.37Z" />
          </g>
        </svg>
      </router-link>
  
      <div class="menu">
        <button class="menu-btn" @click="toogleMenu">
          <i v-if="!isMenuVisible" class="icon-bars"></i>
          <i v-else class="icon-times"></i>
        </button>
  
        <div class="menu-overlay" :data-show="isMenuVisible" @click.self="toogleMenu">
          <div class="menu-panel">
            <img class="menu-logo" src="@/assets/logo/logo-2.svg" alt="logo" />
  
            <div class="menu-list">
              <router-link :to="{ path: '/', hash :'#about'}" class="menu-link" @click.self="toogleMenu">Quienes Somos?</router-link>
              <router-link :to="{ path: '/', hash :'#jobs'}" class="menu-link" @click.self="toogleMenu">Empleos</router-link>
              <router-link :to="{ path: '/', hash :'#recruit'}" class="menu-link" @click.self="toogleMenu">Reclutar</router-link>
              <router-link :to="{ path: '/', hash :'#contact'}" class="menu-link" @click.self="toogleMenu">Contacto</router-link>
            </div>
  
            <div class="menu-footer">
              <SocialLinks />
            </div>
          </div>
        </div>
      </div>
  
      <div class="alter-menu">
        <router-link :to="{ path: '/', hash :'#about'}" class="alter-menu-link">Quienes Somos?</router-link>
        <router-link :to="{ path: '/', hash :'#jobs'}" class="alter-menu-link">Empleos</router-link>
        <router-link :to="{ path: '/', hash :'#recruit'}" class="alter-menu-link">Reclutar</router-link>
        <router-link :to="{ path: '/', hash :'#contact'}" class="alter-menu-link">Contacto</router-link>
      </div>
    </div>
  </div>
</template>

<script>
import { onBeforeUnmount, onMounted, ref, watch } from "vue"
import SocialLinks from "../nav/SocialLinks.vue"

export default {
  name: "Header",
  setup() {
    const isMenuVisible = ref(false);
    const isScrollingUp = ref(true);
    let scrollPos = 0;

    onMounted(() => {
      addEventListener("scroll", handlerScroll);
    });
    onBeforeUnmount(() => {
      removeEventListener("scroll", handlerScroll);
    });


    const handlerScroll = () => {
      if (isMenuVisible.value) return
      if ( window.innerHeight + 10 >= document.body.getBoundingClientRect().bottom ) 
        return isScrollingUp.value = true
      isScrollingUp.value = document.body.getBoundingClientRect().top >= scrollPos && !isMenuVisible.value ? true : false;
      scrollPos = document.body.getBoundingClientRect().top;
    };


    const disableScroll = () => {
      window.onscroll = function () { window.scrollTo(0, window.screenY) };
    }
    // Show/hide the menu panel
    const toogleMenu = () => {
      isMenuVisible.value = !isMenuVisible.value;
    };
    watch(isMenuVisible, newVal => {
      if (newVal) return addEventListener('scroll', disableScroll)
      removeEventListener('scroll', disableScroll)
      window.onscroll = null
    });
    return {
      isScrollingUp,
      isMenuVisible,
      toogleMenu,
    };
  },
  components: { SocialLinks }
}
</script>

<style lang="scss">

.cls-1 {
  fill: url(#Degradado_sin_nombre_2);
}

.cls-2 {
  fill: #fff;
  display: none;

  @media(min-width: 420px ) {
    display: initial;
  }
}

.header {
  margin: auto;
  width: min(100%, 1336px);
  display: flex;
  justify-content: space-between;
  align-items: center;

  &-bg {
    padding: 1em 1.5em;
    position: fixed;
    left: 0;
    right: 0;
    top: -80px;
    transition: 
      top 0.2s,
      background-color 0.2s;
    z-index: 5;
    background-color: var(--dark);

    &[data-show="true"] {
      top: 0px;
    }

    .header-logo {
      height: 2.5em;

      & .cls-2 {
        fill: #fff;
      }
    }
  }


}

.menu {
  &-btn {
    background: none;
    border: none;
    font-size: 25px;
    color: #fff;
  }

  &-overlay {
    margin: 0;
    padding: 0;
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    width: 100%;
    transition: opacity 0.2s 0.5s, transform 0s 0.7s;
    opacity: 0;
    transform: translateX(-100%);

    &[data-show="true"] {
      transition: opacity 0.2s 0s, transform 0s 0s;
      opacity: 1;
      transform: translateX(0);

      & > .menu-panel {
        transform: translateX(0);
      }
    }
  }

  &-panel {
    --overlay-width: 90px;

    position: fixed;
    top: 0;
    left: 0;
    transition: transform 0.7s;
    transform: translateX(calc(-100% - var(--overlay-width)));

    padding-top: 1em;
    border-right: 5px solid var(--dark);
    width: min(calc(100% - var(--overlay-width)));
    height: 100vh;
    background-color: rgba(0, 0, 0, 0.8);
    backdrop-filter: blur(2px);
  }

  &-logo {
    max-height: 100px;
    margin-block: 2em;
  }

  &-list {
    padding: 1.5em 0;
    display: flex;
    flex-direction: column;
  }

  &-link {
    font-size: 1.6rem;
    padding-block: 1em;
    color: #fff;
    display: block;
    height: 100%;
    text-decoration: none;
    transition: background-color 0.2s;

    &:hover {
      background-color: rgba(100,100,100,.5);
    }

    // &.router-link-active {
    //   background-color: rgba(100,100,100,.8);
    //   border-right: 5px solid var(--secondary);
    // }
  }

  &-footer {
    width: 100%;
    padding: 1em 0;
    display: flex;
    justify-content: center;
    position: absolute;
    bottom: 1em;
    background-color: var(--dark);
  }

  @media screen and (min-width: 800px) {
    display: none;
  }
}

.alter-menu {
  display: none;

  @media screen and (min-width: 800px) {
    display: flex;
    gap: 0.5em;

    &-link {
      padding: 0.5em;
      color: #fff;
      text-decoration: none;
    }
  }
}
</style>