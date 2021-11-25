<template>
  <div class="grid mx-12 sm:mx-12">
    <!-- Question Listing Item Card -->
    <div
      class="
        bg-white
        rounded-lg
        shadow-sm
        hover:shadow-lg
        duration-500
        px-2
        sm:px-6
        md:px-2
        py-4
        my-3
      "
    >
      <div class="grid grid-cols-12 gap-3">
        <!-- Meta Column -->
        <div class="col-span-0 sm:col-span-2 text-center hidden sm:block">
          <!-- Answer Counts -->
          <!-- View Counts -->
          <img :src="img" :alt="img" class="w-36 h-36 rounded-lg ml-4 my-2" />
          <div class="grid my-3">
            <span class="inline-block font-bold text-xs"> 1213 Vews </span>
          </div>
        </div>

        <!-- Summary Column -->
        <div class="col-span-12 sm:col-start-3 sm:col-end-13 px-3 sm:px-0">
          <div class="grid sm:hidden">
            <div class="flex flex-wrap">
              <div class="mr-2">
                <div class="inline-block font-light capitalize">
                  <i class="uil uil-arrow-circle-up mr-1"></i>
                  <span class="text-sm"> 21 Votes </span>
                </div>
              </div>
              <div class="mr-2">
                <div class="inline-block font-light capitalize">
                  <i class="uil uil-check-circle mr-1"></i>
                  <span class="text-sm"> 21 Answers </span>
                </div>
              </div>
              <div class="mr-2">
                <div class="inline-block">
                  <i class="uil uil-eye mr-1"></i>
                  <span class="text-sm capitalize font-light"> 21 Views </span>
                </div>
              </div>

              <div class="mr-2">
                <div class="inline-block">
                  <i class="uil uil-clock mr-1"></i>
                  <span class="text-sm font-light"> a few mins ago ago </span>
                </div>
              </div>
            </div>
          </div>

          <div class="flex justify-between items-center sm:block">
            <small class="font-light text-gray-600"> a few min ago </small>
          </div>

          <div class="mt-2">
            <a
              href="#"
              class="
                sm:text-sm
                md:text-md
                lg:text-lg
                text-gray-700
                font-bold
                hover:text-green-500
              "
            >
              Praesent at arcu augue. Etiam lectus massa, consequat
            </a>

            <p class="mt-2 text-gray-600 text-sm md:text-md">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora
              expedita dicta totam totam gul koparam doloremque. Excepturi iste
              iusto eos enim reprehenderit nisi, accusamus... expedita dicta
              totam totam gul koparam doloremque. Excepturi iste iusto eos enim
              reprehenderit nisi, accusamus...
            </p>
          </div>

          <!-- Question Labels -->
          <div class="grid grid-cols-2 mt-4 my-auto">
            <!-- Categories  -->
            <div class="col-span-12 lg:col-span-8">
              <a
                href="#"
                class="
                  inline-block
                  rounded-full
                  text-white
                  bg-red-400
                  hover:bg-red-500
                  duration-300
                  text-xs
                  font-bold
                  mr-1
                  md:mr-2
                  mb-2
                  px-2
                  md:px-4
                  py-1
                  opacity-90
                  hover:opacity-100
                "
              >
                Caching
              </a>
              <a
                href="#"
                class="
                  inline-block
                  rounded-full
                  text-white
                  bg-yellow-400
                  hover:bg-yellow-500
                  duration-300
                  text-xs
                  font-bold
                  mr-1
                  md:mr-2
                  mb-2
                  px-2
                  md:px-4
                  py-1
                  opacity-90
                  hover:opacity-100
                "
              >
                RabbitMQ
              </a>
              <a
                href="#"
                class="
                  inline-block
                  rounded-full
                  text-white
                  bg-green-400
                  hover:bg-green-500
                  duration-300
                  text-xs
                  font-bold
                  mr-1
                  md:mr-2
                  mb-2
                  px-2
                  md:px-4
                  py-1
                  opacity-90
                  hover:opacity-100
                "
              >
                Memcached
              </a>
              <a
                href="#"
                class="
                  inline-block
                  rounded-full
                  text-white
                  bg-blue-400
                  hover:bg-blue-500
                  duration-300
                  text-xs
                  font-bold
                  mr-1
                  md:mr-2
                  mb-2
                  px-2
                  md:px-4
                  py-1
                  opacity-90
                  hover:opacity-100
                "
              >
                Redis
              </a>
            </div>

            <!-- User -->
            <div
              class="col-none hidden mr-2 lg:block lg:col-start-9 lg:col-end-12"
            >
              <a href="#" class="flex items-center">
                <img
                  src="https://avatarfiles.alphacoders.com/165/thumb-1920-165285.png"
                  alt="avatar"
                  class="mr-2 w-8 h-8 rounded-full"
                />

                <div class="text-gray-600 font-bold text-sm hover:underline">
                  EgoistDeveloper
                </div>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  props: {
    img: {
      type: String,
      default:
        "https://images.unsplash.com/photo-1518791841217-8f162f1e1131?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60",
    },
  },
}
</script>

<style>
</style>