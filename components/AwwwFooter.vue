<template>
  <footer class="bg-grey-dark inline-block w-full text-center">
    <div class=" lg:mt-8">
      <img src="~/assets/images/footer.png" class="pull-up">
    </div>

    <div class="flex w-full lg:w-1/2 mx-auto -mt-8">
      <div class="flex-1">
        <ul class="list-reset">
          <li class="mb-4"><a href="/privacy-policy" class="text-black hover:text-grey-darker">Privacy Policy</a></li>
          <li class="mb-4"><a href="/terms-of-use" class="text-black hover:text-grey-darker">Terms of Use</a></li>
        </ul>
      </div>
      <div class="flex-1">
        <ul class="list-reset">
          <li class="mb-4"><a href="/posts" class="text-black hover:text-grey-darker">Blog</a></li>
          <li class="mb-4"><a href="/faq" class="text-black hover:text-grey-darker">FAQ</a></li>
        </ul>
      </div>
      <div class="flex-1">
        <ul class="list-reset">
          <li class="mb-4"><a href="mailto:petar@petar.io" class="text-black hover:text-grey-darker">Contact</a></li>
        </ul>
      </div>
    </div>

    <div class="mt-8 p-4 bg-grey-light text-grey font-normal">
      Copyright © {{ (new Date()).getFullYear() }} Awww. All Rights Reserved.
    </div>
  </footer>
</template>

<script>
export default {}
</script>

<style scoped>
.pull-up {
  transform: translateY(-50%);
}
</style>
