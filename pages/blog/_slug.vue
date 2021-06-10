<template>
  <article>
    <articles :author="article.author"></articles>
    <p>Article last updated: {{ formatDate(article.updatedAt) }}</p>
    <div class="pa4 ph7-l georgia mw9-l center">
      <nuxt-content
        :document="article"
        class="f5 f3-ns lh-copy measure georgia"
      />
    </div>
  </article>
</template>
<script>
export default {
  async asyncData({ $content, params }) {
    const article = await $content('articles', params.slug).fetch()
    return { article }
  },
  methods: {
    formatDate(date) {
      const options = { year: 'numeric', month: 'long', day: 'numeric' }
      return new Date(date).toLocaleDateString('en', options)
    },
  },
}
</script>
<style>
.georgia {
  font-family: georgia, serif;
}
.mw9 {
  max-width: 96rem;
}
.pa4 {
  padding: 2rem;
}
.lh-copy {
  line-height: 1.5;
}
.measure {
  max-width: 30em;
}
.f5 {
  font-size: 1rem;
}
.center {
  margin-right: auto;
  margin-left: auto;
}
@media screen and (min-width: 30em) {
  .pt5-ns {
    padding-top: 4rem;
  }
  .f3-ns {
    font-size: 1.5rem;
  }
  @media screen and (min-width: 60em) {
    .mw9-l {
      max-width: 96rem;
    }
    .ph7-l {
      padding-left: 16rem;
      padding-right: 16rem;
    }
  }
}
</style>
