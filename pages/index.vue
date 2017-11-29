<template>
  <div>
    <landing-header></landing-header>

    <awww-section>
      <template slot="highlight">
        <div class="highlight highlight--top-left"></div>
        <div class="highlight highlight--top-right"></div>
      </template>

      <template slot="image">
        <img src="~/assets/images/section1.png" alt="">
      </template>

      <template slot="title">
        Scientifically proven to reduce stress 👩‍🔬
      </template>

      <template slot="content">
        <a href="http://www.sciencealert.com/watching-cat-videos-lowers-stress-and-makes-you-happy-study-reveals">Recent research</a> shows that looking at cute animal pictures 🐼 instantly improves your mood. Cute animal images give you positive vibes 😆 and make you happier by taking only a few minutes a day to enjoy them.
      </template>
    </awww-section>

    <div class="text-2xl lg:text-5xl text-center m-4">😻 🐶 🙊 🐼 🐥 🐙</div>

    <awww-section :alternate="true">
      <template slot="highlight">
        <div class="highlight highlight--bottom-left"></div>
        <div class="highlight highlight--bottom-right"></div>
      </template>

      <template slot="image">
        <img src="~/assets/images/section2.png" alt="">
      </template>

      <template slot="title">
        Happier and Super Productive 😍
      </template>

      <template slot="content">
        Cute animal images trigger production of your “happy hormone” 😂. Apart for making you happy, looking at cute animal images also makes you <a href="http://www.psychologicalscience.org/news/minds-business/the-power-of-puppies-looking-at-cute-images-can-improve-focus.html#.WKBRkhIrJE4">more productive</a>! A perfect combination to help you feel great at work and at home. 💪 🏢 🏠
      </template>
    </awww-section>

    <div class="text-2xl lg:text-5xl text-center m-4">😻 🐶 🙊 🐼 🐥 🐙</div>

    <awww-section>
      <template slot="highlight">
        <div class="highlight highlight--top-left"></div>
        <div class="highlight highlight--top-right"></div>
      </template>

      <template slot="image">
        <img src="~/assets/images/section3.png" alt="">
      </template>

      <template slot="title">
        Set and Forget Scheduling ⌚️
      </template>

      <template slot="content">
        Tell us when you’d like to receive our doses of cuteness and forget about it! We’ll deliver them into your inbox every day at that time, wherever you are. No fuss. All you have to do is enjoy! ✅
      </template>
    </awww-section>

    <testemonials></testemonials>

    <pricing></pricing>

    <br><br><br>

    <blog-posts></blog-posts>

    <subscribe></subscribe>

    <br><br><br><br><br><br><br><br><br><br>

    <awww-footer></awww-footer>
  </div>
</template>

<script>
import LandingHeader from '~/components/LandingHeader.vue'
import AwwwSection from '~/components/AwwwSection.vue'
import Testemonials from '~/components/Testemonials.vue'
import Pricing from '~/components/Pricing.vue'
import Subscribe from '~/components/Subscribe.vue'
import AwwwFooter from '~/components/AwwwFooter.vue'
import BlogPosts from '~/components/BlogPosts.vue'

export default {
  components: {
    LandingHeader,
    AwwwSection,
    Testemonials,
    Pricing,
    Subscribe,
    AwwwFooter,
    BlogPosts
  }
}
</script>

<style>
</style>
