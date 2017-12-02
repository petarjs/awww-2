<template>
  <section class="lg:mb-8 text-center">
    <div class="text-center mt-8 pt-8 mb-8">
      <div class="text-3xl mb-4">🌟 🌟 🌟 🌟 🌟</div>
      <h2 class="text-medium text-5xl">Plans and Pricing ✅</h2>
    </div>

    <div class="container mx-auto p-2 lg:mt-4 inline-block">
      <div class="flex flex-wrap p-2 lg:p-0">
        <div class="text-center border border-grey-light rounded-lg lg:flex-1 flex-no-shrink lg:flex-shrink min-w-full w-full lg:w-auto lg:min-w-0 lg:mx-2 mb-6 lg:mb-0">
          <div class="text-4xl font-bold p-8 border-b">
            Kitty 🐱
          </div>
          <div class="bg-grey-darkest p-4 text-white">
            <span class="text-5xl font-medium">FREE</span>
          </div>
          <div class="text-lg font-light p-4 border-b">
            Email Newsletter ✅
          </div>
          <div class="text-lg font-light p-4 border-b">
            Custom Scheduling ✅
          </div>
          <div class="text-lg font-light p-4 border-b">
            <span class="font-bold">1</span> Email / Day ✅
          </div>
          <div class="text-lg font-light p-4 border-b">
            Only Images ✅
          </div>
          <div class="text-lg font-light p-8">
            <a href="#" @click.prevent="onBuy" class="font-medium p-3 bg-green text-white rounded-lg hover:text-white hover:bg-green-light">Get it now!</a>
          </div>
        </div>

      <div class="text-center border border-grey-light rounded-lg lg:flex-1 flex-no-shrink lg:flex-shrink min-w-full w-full lg:w-auto lg:min-w-0 lg:mx-2 mb-6 lg:mb-0">
          <div class="text-4xl font-bold p-8 border-b">
            Tiger 🐯
          </div>
          <div class="bg-yellow-dark p-4 text-white">
            <span class="text-5xl font-medium">$3.99</span> / month
          </div>
          <div class="text-lg font-light p-4 border-b">
            Email Newsletter ✅
          </div>
          <div class="text-lg font-light p-4 border-b">
            Custom Scheduling ✅
          </div>
          <div class="text-lg font-light p-4 border-b">
            <span class="font-bold">1</span> Email / Day ✅
          </div>
          <div class="text-lg font-light p-4 border-b">
            Images &amp; Videos ✅
          </div>
          <div class="text-lg font-light p-8">
            <a href="#" @click.prevent="onBuy" class="font-medium p-3 bg-green text-white rounded-lg hover:text-white hover:bg-green-light">Get it now!</a>
          </div>
        </div>

      <div class="text-center border border-grey-light rounded-lg lg:flex-1 flex-no-shrink lg:flex-shrink min-w-full w-full lg:w-auto lg:min-w-0 lg:mx-2 mb-6 lg:mb-0">
          <div class="text-4xl font-bold p-8 border-b">
            Lion 🦁
          </div>
          <div class="bg-grey-darkest p-4 text-white">
            <span class="text-5xl font-medium">$19.99</span> / month
          </div>
          <div class="text-lg font-light p-4 border-b">
            Email Newsletter ✅
          </div>
          <div class="text-lg font-light p-4 border-b">
            Custom Scheduling ✅
          </div>
          <div class="text-lg font-light p-4 border-b">
            <span class="font-bold">Up to 10 Emails / Day</span> ✅
          </div>
          <div class="text-lg font-light p-4 border-b">
            Images &amp; Videos ✅
          </div>
          <div class="text-lg font-light p-8">
            <a href="#" @click.prevent="onBuy" class="font-medium p-3 bg-green text-white rounded-lg hover:text-white hover:bg-green-light">Get it now!</a>
          </div>
        </div>
      </div>
    </div>

    <!--<div class="container mx-auto px-4 py-2">
      <a href="#" class="w-full max-w-full inline-block text-center text-lg border border-grey-light hover:border-orange-light rounded-lg p-4">
        Company? We've got special packages for you! 👌
      </a>
    </div>-->
    <div class="container mx-auto px-4 py-2">
      <div class="w-full max-w-full inline-block text-center text-lg border border-grey-light rounded-lg p-4">
        Company? Special packages for you comming soon! 👌
      </div>
    </div>

  </section>
</template>

<script>
import bus from '~/services/bus'
export default {
  components: {},
  methods: {
    onBuy () {
      bus.$emit('pricing:show-subscribe')
    }
  }
}
</script>

<style scoped>
.pull-up {
  transform: translateY(-50%);
}

.pull-up-sm {
  transform: translateY(-23px);
}
</style>
