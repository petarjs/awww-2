<template>
  <section class="bg-yellow-dark text-center subscribe" ref="subscribePromo">
    <div class="text-center mt-8 pt-8 mb-8">
      <h2 class="text-medium text-5xl">Get Started Today 📅</h2>
    </div>

    <div class="container mx-auto p-2 lg:mt-4 inline-block text-2xl leading-normal font-light">
      There's so much <span class="font-medium">cuteness</span> all around us. <br>
      Take a moment <span class="font-medium">every day</span> to enjoy it.
    </div>

    <div class="mt-4 lg:mt-8 pl-4 pr-4 lg:pr-0 mx-auto">
      <form action="https://ooo.us17.list-manage.com/subscribe/post?u=eade1f006b2b21eba3732d565&amp;id=e7c7f92710" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
        <input name="EMAIL" class="rounded-lg border border-dark-grey p-2 pl-4 pr-4 lg:p-4 w-full lg:w-64 lg:text-lg leading-loose lg:leading-normal" type="email" placeholder="Your Email 💌">
        <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_eade1f006b2b21eba3732d565_e7c7f92710" tabindex="-1" value=""></div>
        <button type="submit" name="subscribe" class="rounded-lg bg-green hover:bg-green-light p-4 lg:p-4 mt-2 lg:mt-0 lg:-ml-2 text-white lg:text-lg lg:leading-normal">Get Your Invite 💪</button>
      </form>
    </div>

    <span v-if="showSubscribe" class="p-4 border border-green mx-4 lg:mx-auto rounded-lg inline-block mt-8 text-green">
      Please enter your email here and we'll notify you when we launch Awww! 🎁
    </span>
  </section>
</template>

<script>
import bus from '~/services/bus'
import Vue from 'vue'

export default {
  data () {
    return {
      showSubscribe: false
    }
  },
  created () {
    bus.$on('pricing:show-subscribe', this.onShowSubscribe.bind(this))
  },
  destroyed () {
    bus.$off('pricing:show-subscribe')
  },
  methods: {
    onShowSubscribe () {
      this.showSubscribe = true
      Vue.nextTick(() => {
        let container = this.$refs.subscribePromo
        window.scroll(0, container.offsetTop - 10)
      })
    }
  },
  components: {}
}
</script>

<style scoped>
.subscribe {
  padding-bottom: 180px;
  padding-top: 20px;
}
</style>
