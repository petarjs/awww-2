<template>
  <div>
    <div class="container mx-auto p-4 lg:p-8">
      <div class="column text-center mb-6 mt-6">
          <a href="/">
              <img src="~/assets/images/logo-dark.png" alt="" width="200px">
          </a>
      </div>

      <section class="lg:mb-8 text-center">
        <div class="text-center mt-8 pt-8 mb-8">
          <h2 class="text-medium text-5xl">From our Blog ✒️</h2>
        </div>

        <div class="container mx-auto p-2 lg:mt-4 inline-block text-2xl leading-normal font-light">
          <a v-for="post in blogPostList" :key="post.title" class="m-2 inline-block text-black hover:text-orange" :href="post.link">
            <div class="max-w-sm rounded overflow-hidden shadow-lg mx-auto">
              <img class="w-full" :src="post.image">
              <div class="px-6 py-4">
                <div class="font-bold text-xl mb-2">{{ post.title }}</div>
                <p class="text-grey-darker text-base">
                  {{ post.desc }}
                </p>
              </div>
              <div class="px-6 py-4">
                <span v-for="tag in post.tags" :key="tag" class="inline-block bg-grey-lighter rounded-full px-3 py-1 text-sm font-semibold text-grey-darker mr-2">#{{ tag }}</span>
              </div>
            </div>
          </a>
        </div>
      </section>
    </div>
    <div>
      <br><br><br><br><br><br><br><br><br><br>
      <awww-footer></awww-footer>
    </div>
  </div>
</template>
<script>
import AwwwFooter from '~/components/AwwwFooter.vue'
import blogPostList from '~/services/blogPostList'

export default {
  data () {
    return {
      blogPostList
    }
  },
  computed: {
  },
  components: {
    AwwwFooter
  }
}
</script>
<style>
</style>
