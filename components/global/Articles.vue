<template>
  <article>
    <header class="bg-gold sans-serif">
      <div class="mw9 center pa4 pt5-ns ph7-l">
        <time class="f6 mb2 dib ttu tracked"
          ><small>{{ author.date }}</small></time
        >
        <h3 class="f2 f1-m f-headline-l measure-narrow lh-title mv0">
          <span class="bg-black-90 lh-copy white pa1 tracked-tight">
            {{ author.title }}
          </span>
        </h3>
        <h4 class="f3 fw1 georgia i">
          {{ author.subtitle }}
        </h4>
        <h5 class="f6 ttu tracked black-80">By {{ author.name }}</h5>
      </div>
    </header>
    <div class="pa4 ph7-l georgia mw9-l center">
      <p class="f5 f3-ns lh-copy measure georgia">
        Theodore Sturgeon was a science fiction author, critic, and the basis
        for Kurt Vonnegut's recurring character Kilgore Trout. He was prolific,
        authoring over 200 pieces himself and critiquing around 400 others.
      </p>
      <p class="f5 f3-ns lh-copy measure georgia">
        In 1958 he published a piece in Venture proclaiming what he called
        "Sturgeon's Revelation"
      </p>
      <p class="f6 f5-ns lh-copy measure i pl4 bl bw1 b--gold mb4">
        I repeat Sturgeon's Revelation, which was wrung out of me after twenty
        years of wearying defense of science fiction against attacks of people
        who used the worst examples of the field for ammunition, and whose
        conclusion was that ninety percent of SF is crud. Using the same
        standards that categorize 90% of science fiction as trash, crud, or
        crap, it can be argued that 90% of film, literature, consumer goods,
        etc. is crap. In other words, the claim (or fact) that 90% of science
        fiction is crap is ultimately uninformative, because science fiction
        conforms to the same trends of quality as all other artforms.
      </p>
      <p class="f5 f4-ns lh-copy measure mb4"></p>

      <p class="f5 f4-ns lh-copy measure"></p>
    </div>
  </article>
</template>
<script>
export default {
  props: {
    author: {
      type: Object,
      required: true,
    },
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
.bl {
  border-left-style: solid;
  border-left-width: 1px;
}

.b--gold {
  border-color: #ffb700;
}

.bw1 {
  border-width: 0.125rem;
}

.dib {
  display: inline-block;
}

.sans-serif {
  font-family: -apple-system, BlinkMacSystemFont, 'avenir next', avenir,
    'helvetica neue', helvetica, ubuntu, roboto, noto, 'segoe ui', arial,
    sans-serif;
}

.georgia {
  font-family: georgia, serif;
}

.i {
  font-style: italic;
}

.fw1 {
  font-weight: 100;
}

.tracked {
  letter-spacing: 0.1em;
}

.tracked-tight {
  letter-spacing: -0.05em;
}

.lh-title {
  line-height: 1.25;
}

.lh-copy {
  line-height: 1.5;
}

.mw9 {
  max-width: 96rem;
}

.black-80 {
  color: rgba(0, 0, 0, 0.8);
}

.white {
  color: #fff;
}

.bg-black-90 {
  background-color: rgba(0, 0, 0, 0.9);
}

.bg-gold {
  background-color: #ffb700;
}

.pa1 {
  padding: 0.25rem;
}

.pa4 {
  padding: 2rem;
}

.pl4 {
  padding-left: 2rem;
}

.mb2 {
  margin-bottom: 0.5rem;
}

.mb4 {
  margin-bottom: 2rem;
}

.mv0 {
  margin-top: 0;
  margin-bottom: 0;
}

.ttu {
  text-transform: uppercase;
}

.f2 {
  font-size: 2.25rem;
}

.f3 {
  font-size: 1.5rem;
}

.f5 {
  font-size: 1rem;
}

.f6 {
  font-size: 0.875rem;
}

.measure {
  max-width: 30em;
}

.measure-narrow {
  max-width: 20em;
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

  .f4-ns {
    font-size: 1.25rem;
  }

  .f5-ns {
    font-size: 1rem;
  }
}

@media screen and (min-width: 30em) and (max-width: 60em) {
  .f1-m {
    font-size: 3rem;
  }
}

@media screen and (min-width: 60em) {
  .mw9-l {
    max-width: 96rem;
  }

  .ph7-l {
    padding-left: 16rem;
    padding-right: 16rem;
  }

  .f-headline-l {
    font-size: 6rem;
  }
}
</style>
