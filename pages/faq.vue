<template>
  <div>
    <div class="container mx-auto p-4 lg:p-8">
      <div class="column text-center mb-6 mt-6">
          <a href="/">
              <img src="~/assets/images/logo-dark.png" alt="" width="200px">
          </a>
      </div>
      <div class="flex flex-col lg:flex-row sm:p-4 lg:p-8 lg:my-4 max-w-xl justify-center items-center ml-auto mr-auto">
        <div class="flex-1 sm:p-4 lg:p-8">
          <h1 class="leading-normal text-center lg:text-left text-4xl mb-8 font-medium awww-section__title">FAQ</h1>

          <h2 class="leading-normal text-center lg:text-left text-2xl mb-8 font-medium awww-section__title">
            What will I get when I sign up?
          </h2>
          <p class="leading-normal text-lg font-light awww-section__content mb-8">
            You will receive an email every day containing handpicked cute animal images, gifs and videos.
          </p>

          <h2 class="leading-normal text-center lg:text-left text-2xl mb-8 font-medium awww-section__title">
            Which animals do you send?
          </h2>
          <p class="leading-normal text-lg font-light awww-section__content mb-8">
            Almost all animals can be super cute! Cats, dogs, foxes, monkeys, pandas, koalas, red pandas... You name it! 😻 🐶 🙊 🐼 🐥 🐙
          </p>

          <h2 class="leading-normal text-center lg:text-left text-2xl mb-8 font-medium awww-section__title">
            Why would I want to get cute images in an email every day?
          </h2>
          <p class="leading-normal text-lg font-light awww-section__content mb-8">
            Because looking at cute animal images is a research proven way to reduce stress and increase producitivty. It's a perfect way to take a few minutes and relax at work.
          </p>

          <h2 class="leading-normal text-center lg:text-left text-2xl mb-8 font-medium awww-section__title">
            Can I set the time when I get the cute images?
          </h2>
          <p class="leading-normal text-lg font-light awww-section__content mb-8">
            Yes. You will be able to set your preferred time and timezone when you'll get the wonderful, stress reducing images.
          </p>

          <h2 class="leading-normal text-center lg:text-left text-2xl mb-8 font-medium awww-section__title">
            Will my boss get mad because I'm looking at cute images?
          </h2>
          <p class="leading-normal text-lg font-light awww-section__content mb-8">
            Probably not. It will only take a few minutes of your day, and give you benefits of increased productivity. If anything, you should recommend this service to your boss as well!
          </p>

          <h2 class="leading-normal text-center lg:text-left text-2xl mb-8 font-medium awww-section__title">
            Is there a Free Plan?
          </h2>
          <p class="leading-normal text-lg font-light awww-section__content mb-8">
            Yes, a Free Tier including only images will be available.
          </p>

          <h2 class="leading-normal text-center lg:text-left text-2xl mb-8 font-medium awww-section__title">
            What if I don't like the what I'm getting?
          </h2>
          <p class="leading-normal text-lg font-light awww-section__content mb-8">
            We will refund you in full in 30 after purchase.
          </p>

          <h2 class="leading-normal text-center lg:text-left text-2xl mb-8 font-medium awww-section__title">
            What if I absolutely love this service?
          </h2>
          <p class="leading-normal text-lg font-light awww-section__content mb-8">
            Please share it with your friends and make their day brighter too! :)
          </p>

        </div>
      </div>
    </div>
    <div>
      <br><br><br><br><br><br><br><br><br><br>
      <awww-footer></awww-footer>
    </div>
  </div>
</template>

<script>
import AwwwFooter from '~/components/AwwwFooter.vue'

export default {
  components: {
    AwwwFooter
  }
}
</script>

<style>

a {
  color: #f6993f;
  text-decoration: none;
}

input {
  outline: none;
}

a:hover {
  color: orange;
}

</style>
