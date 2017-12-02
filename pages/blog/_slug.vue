<template>
  <div>
    <div class="container mx-auto p-4 lg:p-8">
      <div class="column text-center mb-6 mt-6">
          <a href="/">
              <img src="~/assets/images/logo-dark.png" alt="" width="200px">
          </a>
      </div>

      <div class="flex flex-col lg:flex-row sm:p-4 lg:p-8 my-4 max-w-xl justify-center items-center ml-auto mr-auto">
        <div class="flex-1 sm:p-4 lg:p-8">
          <h1 class="title leading-normal text-center lg:text-left text-4xl mb-8 font-medium awww-section__title">{{ title }}</h1>
          <img src="https://tailwindcss.com/img/card-top.jpg" alt="">
        </div>
      </div>

      <div class="lg:w-2/3 mx-auto leading-normal text-lg">
        <p class="mb-8 pb-4">
          We all get unhappy sometimes. The burden of everyday life, our responsibilities and chores can come crashing down on us hard. Sometimes it's a brief episode, and sometimes the low feeling lasts a long, long time. In today's world of stress, constant struggle with time and energy, we all need a few life hacks to make us happier. Here is a list of 7 practical things you can start doing right now and feel immediate benefits.
        </p>

        <h2 class="mb-4">
          1. Buy yourself some time
        </h2>
        <p class="mb-8 pb-4">If you think about it, time is our most precious resource, by far. This is especially true if you are living a hectic life - working long hours or having many chores that drain your energy and leave you with little time to relax and do what makes you feel good. <a href="http://www.bbc.com/news/science-environment-40703519">Recent study</a> shows that using money to free up your time is the greatest contributor to happiness. So next time when you're feeling down, order takeout instead of cooking or hire a cleaner instead of cleaning the house yourself!</p>

        <h2 class="mb-4">
          2. Look at cute animal images
        </h2>
        <p class="mb-8 pb-4">Rejoice! This one is awesome. There are studies that show that looking at cute animal images daily <a href="http://www.independent.co.uk/life-style/health-and-families/features/why-cute-photos-of-animals-make-us-happier-10332916.html">increases happiness</a> and <a href="http://www.sciencealert.com/watching-cat-videos-lowers-stress-and-makes-you-happy-study-reveals">reduces stress</a>. Imagine having a tough workday, taking a minute to look at some cute animals and instantly feeling better! <a href="https://awww.ooo">Awww</a> offers to send you daily doses of cuteness in form of images and videos via email so you can get happier every day.</p>

        <h2 class="mb-4">
          3. Stretch
        </h2>
        <p class="mb-8 pb-4">Sounds weird? Don't be fooled, stretching first thing in the morning while you're still in your bed significantly improves <a href="https://www.mamamia.com.au/stretching-in-the-morning/">mood and confidence</a>. For an even better effect, nicely stretch when you go to bed at night too. It really feels great! Another time you can practice this happiness booster is during work. Every few hours take a minute to stretch. It's like a mini office workout! When you go to bed tonight, remember to try and stretch. You'll feel better immediately.</p>

        <h2 class="mb-4">
          4. Hug more (and longer)
        </h2>
        <p class="mb-8 pb-4">Numerous studies show us that human touch is essential for our well being. We best bond with other people through touch. Of all the ways we can touch, hugs (especially long ones) are unique because they cause us to release <a href="http://theweek.com/articles/646192/science-how-touch-makes-happier">a lot of oxytocin</a> - a chemical that makes us bond with a person and makes us feel good. How much hugging should you aim for? There's no exact number, but at least 5 hugs a day sounds like a good idea. Go out there and hug your kids, your partner, your friends and your coworkers!</p>

        <h2 class="mb-4">
          5. Dance (Alone)
        </h2>
        <p class="mb-8 pb-4">Did you know that dancing <a href="http://www.telegraph.co.uk/good-news/seven-seas/why-dancing-feels-good/">reduces cortisol</a>? And it also makes you happy by releasing <a href="https://psychology-spot.com/dancing-makes-me-happy/">endorphins</a>. Dancing is awesome, but in our civilisation it's reserved for special occasions. Just getting up an starting dancing might get you strange looks from the people around you. You might also feel uncomfortable dancing to your fulest around others if you are an introvert. So try getting alone, lock the door, play some music you love and start dancing like no one is watching! You'll feel great!</p>

        <h2 class="mb-4">
          6. Listen to sad music
        </h2>
        <p class="mb-8 pb-4">While it may sound contradictory, <a href="http://www.huffingtonpost.com/entry/why-we-like-sad-music_us_562a52a8e4b0aac0b8fc9e99">study</a> shows that sad music helps us feel better by boosting positive feelings. It also makes us feel catharsis, providing an emotional release. In a busy world, we often overlook how many negative emotions we have bottled up, and getting them released feels powerful and healing.</p>

        <h2 class="mb-4">
          7. Give a massage
        </h2>
        <p class="lg:mb-8 pb-4">When you imagine a massage, the first thing that comes to mind is that the only one enjoying it is the one receiving it. But that's not exactly true. <a href="https://www.medicalnewstoday.com/articles/317315.php">Recent research</a> has found that when you give a massage, you get the same stress reducing benefits that receiving a massage so famously has. It's the magic of human touch. If you're massaging your partner or a friend, all that touching creates a bonding experience and <a href="http://www.hugthemonkey.com/2008/07/finally-massage-increases-oxytocin.html">releases oxytocin</a>. Another way you can de-stress is if your  massage partner enjoys rough massages. You can then energetically rub, squish and knead until all the negative energy is out!</p>
      </div>

    </div>

    <div class="lg:mb-8"></div>

    <subscribe></subscribe>

    <br><br><br><br><br><br><br><br><br><br>

    <awww-footer></awww-footer>
  </div>
</template>
<script>
import Subscribe from '~/components/Subscribe.vue'
import AwwwFooter from '~/components/AwwwFooter.vue'

export default {
  computed: {
    title () {
      return this.$route.params.slug.replace(/-/g, ' ')
    }
  },
  components: {
    Subscribe,
    AwwwFooter
  }
}
</script>
<style>
  .title {
    text-transform: capitalize
  }
</style>
