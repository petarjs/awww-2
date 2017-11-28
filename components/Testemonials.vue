<template>
  <section class="cover bg-cover bg-center lg:mb-8">
    <div class="m-8">
      <div class="lg:ml-4 lg:mt-8 pt-8">
        <h2 class="text-left text-4xl text-white font-medium leading-normal">People are loving Awww ❤️</h2>
      </div>

      <div class="lg:mt-8">
        <div class="flex flex-wrap lg:w-2/3">
          <a href="#" class="w-full lg:w-64 lg:m-4 lg:mb-8 mt-8 flex-no-shrink" v-for="i in [1,2,3,4,5,6]">
            <div class="p-8 bg-white rounded leading-normal text-black mb-4">
              Awww is the best! Since I've been using it, I have been feeling wonderful!
            </div>
            <div class="flex items-center">
              <img class="w-16 h-16 rounded-full mr-4" src="~/assets/images/avatar.png" alt="Avatar">
              <div class="text-xl text-left">
                <p class="text-white">Petar Slovic</p>
                <p class="text-grey-light">via Twitter</p>
              </div>
            </div>
          </a>
        </div>
      </div>

    </div>
  </section>
</template>

<script>
export default {
  components: {}
}
</script>

<style scoped>
.cover {
  background-image: url("~/assets/images/testemonial-puppy.jpg");
  min-height: 100vh;
  display: flex;
  justify-content: start;
  align-items: start;
  text-align: center;
}
</style>
