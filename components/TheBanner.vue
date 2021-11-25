<template>
  <section
    class="
      grid grid-cols-3
      container
      mx-auto
      gap-4
      rounded-lg
      p-4
      pt-24
      bg-white
    "
  >
    <div class="col-span-2 row-span-2">
      <div class="relative pt-[56.25%] overflow-hidden">
        <div>
          <img
            class="absolute inset-0 w-full h-full object-cover"
            src="https://picsum.photos/id/19/500/800"
            alt=""
          />
        </div>
      </div>

      <h3 class="mt-2 text-lg truncate uppercase tracking-wider">
        Lorem Ipsum
      </h3>
    </div>

    <div class="relative">
      <div class="relative pt-[56.25%] overflow-hidden">
        <img
          class="absolute inset-0 w-full h-full object-cover"
          src="https://picsum.photos/id/14/500/800"
          alt=""
        />
      </div>

      <h3
        class="
          absolute
          inset-x-0
          bg-white
          bottom-0
          pt-2
          text-lg
          truncate
          uppercase
          tracking-wider
        "
      >
        Dolor Sit Amet
      </h3>
    </div>

    <div class="relative">
      <div class="relative pt-[56.25%] overflow-hidden">
        <img
          class="absolute inset-0 w-full h-full object-cover"
          src="https://picsum.photos/id/18/500/800"
          alt=""
        />
      </div>

      <h3
        class="
          absolute
          inset-x-0
          bg-white
          bottom-0
          pt-2
          text-lg
          truncate
          uppercase
          tracking-wider
        "
      >
        Blog 2 Title here
      </h3>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style>
.pt-\[56\.25\%\] {
  padding-top: 56.25%;
}
</style>