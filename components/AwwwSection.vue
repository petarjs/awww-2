<template>
  <section class="relative mt-8 mb-8 lg:mb-0 lg:mt-8 overflow-hidden">
    <slot name="highlight"></slot>

    <div class="container mx-auto p-4 lg:p-8" v-if="alternate">
      <div class="flex flex-col lg:flex-row sm:p-4 lg:p-8 lg:my-4 max-w-xl justify-center items-center ml-auto mr-auto">
        <div class="p-8 sm:block lg:hidden" v-if="true">
          <slot name="image"></slot>
        </div>
        <div class="flex-1 lg:p-8">
          <h2 class="leading-normal text-center lg:text-left mb-8 font-medium awww-section__title"><slot name="title"></slot></h2>
          <p class="leading-normal text-lg font-light awww-section__content"><slot name="content"></slot></p>
        </div>
        <div class="p-8 lg:block hidden">
          <slot name="image"></slot>
        </div>
      </div>
    </div>
    <div class="container mx-auto p-4 lg:p-8" v-else>
      <div class="flex flex-col lg:flex-row sm:p-4 lg:p-8 lg:my-4 max-w-xl justify-center items-center ml-auto mr-auto">
        <div class="p-8">
          <slot name="image"></slot>
        </div>
        <div class="flex-1 sm:p-4 lg:p-8">
          <h2 class="leading-normal text-center lg:text-left text-4xl mb-8 font-medium awww-section__title"><slot name="title"></slot></h2>
          <p class="leading-normal text-lg font-light awww-section__content"><slot name="content"></slot></p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: ['alternate']
}
</script>

<style>
.awww-section__title {
  font-size: 2.5rem;
}

.awww-section__content {
  font-size: 1.2rem;
}

@media screen and (max-width: 992px) {
  .awww-section__title {
    font-size: 2rem;
  }
}
</style>

