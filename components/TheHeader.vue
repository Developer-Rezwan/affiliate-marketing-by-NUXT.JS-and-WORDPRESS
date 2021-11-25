<template>
  <div class="fixed w-full">
    <nav class="flex items-center bg-gray-600 p-3 flex-wrap sticky w-full">
      <a href="#" class="p-2 mr-4 inline-flex items-center">
        <img
          src="/public/images/meta-icon-new-facebook-2021-seeklogo.com-2.svg"
          class="w-8 mr-1"
        />
        <span class="text-xl text-white font-bold uppercase tracking-wide"
          >Metaverse</span
        >
      </a>
      <button
        @click="isOpen = !isOpen"
        class="
          text-white
          inline-flex
          p-3
          hover:bg-gray-900
          rounded
          lg:hidden
          ml-auto
          hover:text-white
          outline-none
          nav-toggler
        "
      >
        <i class="material-icons">menu</i>
      </button>
      <div
        v-if="isOpen"
        class="
          top-navbar
          w-full
          lg:inline-flex lg:flex-grow lg:w-auto
          md:right-0
          lg:right-0
        "
      >
        <div
          class="
            lg:inline-flex lg:flex-row lg:ml-auto lg:w-auto
            w-full
            lg:items-center
            items-start
            flex flex-col
            lg:h-auto
          "
        >
          <NuxtLink
            v-for="route in routers"
            :key="route.name"
            :to="route.url"
            class="
              lg:inline-flex lg:w-auto
              w-full
              px-3
              py-2
              rounded
              text-gray-400
              items-center
              justify-center
              hover:bg-gray-900 hover:text-white
            "
          >
            <span>{{ route.name }}</span>
          </NuxtLink>
        </div>
      </div>
    </nav>
  </div>
</template>

<script lang="js">
export default {
  data() {
    return {
      isOpen: true,
      routers: [
        {
          name: "Home",
          url: "/",
        },
        {
          name: "About",
          url: "/about",
        },
        {
          name: "Contact",
          url: "/contact",
        },
      ],
    }
  },

  mounted() {
    this.responsive()
  },

  methods: {
    /* responsive screen */
    responsive() {
      window.addEventListener("resize", () => {
        if (window.innerWidth > 1023) {
          this.isOpen = true
        } else {
          this.isOpen = false
        }
      })
    },
  },
}
</script>

<style>
@import url("https://cdnjs.cloudflare.com/ajax/libs/material-design-icons/3.0.1/iconfont/material-icons.min.css");
@import url("https://fonts.googleapis.com/css2?family=Rubik:wght@300;400;500;700;900&display=swap");
html,
body {
  font-family: "Rubik", sans-serif;
}

/* navigation 
 - show navigation always on the large screen devices with (min-width:1024)
*/
.router-link-active {
  --tw-bg-opacity: 1;
  background-color: rgba(17, 24, 39, var(--tw-bg-opacity));
  --tw-text-opacity: 1;
  color: rgba(255, 255, 255, var(--tw-text-opacity));
}

@media (min-width: 1024px) {
  .top-navbar {
    display: inline-flex !important;
  }
}
</style>