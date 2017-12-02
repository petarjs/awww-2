<template>
  <section class="cover--cat bg-cover bg-center lg:mb-8">
    <div class="flex flex-col justify-center lg:h-screen w-screen overflow-hidden">
      <div class="lg:text-left mt-2 lg:mt-8 lg:ml-8 lg:pl-8">
        <logo/>
      </div>

      <div class="lg:ml-8 lg:pl-8 mt-4 lg:mt-8 text-3xl lg:text-5xl font-semibold text-white lg:text-left">
        <div class="pt-3 pl-3 pr-3 pb-1 bg-black-transparent inline-block">STRESS DOWN<span class="text-orange">.</span></div>
        <br>
        <div class="pb-3 pl-3 pr-3 pt-1 bg-black-transparent inline-block"><span class="text-orange">PRODUCTIVITY</span> UP.</div>
      </div>

      <div class="lg:pl-8">
        <div class="ml-4 mr-4 lg:ml-8 lg:mr-0 mt-4 lg:mt-8 bg-black-transparent text-white text-xl lg:text-2xl leading-normal text-left w-500 p-3">
          <a href="http://www.sciencealert.com/watching-cat-videos-lowers-stress-and-makes-you-happy-study-reveals">De-stress</a> and <a href="http://www.independent.co.uk/life-style/health-and-families/features/why-cute-photos-of-animals-make-us-happier-10332916.html">increase happiness</a> with our lovingly
          handpicked images and videos of cutest animals that arrive in your email inbox every day.
        </div>
      </div>

      <div class="lg:ml-8 lg:pl-8 mt-4 lg:mt-8 lg:text-left pl-4 pr-4 lg:pr-0">
        <form action="https://ooo.us17.list-manage.com/subscribe/post?u=eade1f006b2b21eba3732d565&amp;id=e7c7f92710" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
          <input name="EMAIL" class="rounded border-0 p-2 pl-4 pr-4 lg:p-4 w-full lg:w-64 lg:text-lg leading-loose lg:leading-normal" type="email" placeholder="Your Email 💌">
          <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_eade1f006b2b21eba3732d565_e7c7f92710" tabindex="-1" value=""></div>
          <button type="submit" name="subscribe" class="rounded bg-green hover:bg-green-light p-4 lg:p-4 mt-2 lg:mt-0 lg:-ml-2 text-white lg:text-lg lg:leading-normal">Get Your Invite 💪</button>
        </form>
      </div>

      <div class="text-white mt-2 mb-2 lg:mt-4 lg:ml-8 lg:pl-8 lg:text-left">
        * we promise we'll never spam you
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.cover--cat {
  background-image: url("~/assets/images/cat.jpg");
  min-height: 100vh;
  display: flex;
  justify-content: start;
  align-items: start;
  text-align: center;
}

.bg-black-transparent {
  background-color: rgba(0, 0, 0, 0.7);
}

</style>

