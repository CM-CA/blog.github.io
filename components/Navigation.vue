<template>
  <header class="bg-white black-80 tc pv4 avenir">
    <a href="" class="bg-black-80 ba b--black dib pa3 w2 h2 br-100">
      <svg
        class="white"
        data-icon="skull"
        viewBox="0 0 32 32"
        style="fill: currentcolor"
      >
        <title>skull icon</title>
        <path
          d="M16 0 C6 0 2 4 2 14 L2 22 L6 24 L6 30 L26 30 L26 24 L30 22 L30 14 C30 4 26 0 16 0 M9 12 A4.5 4.5 0 0 1 9 21 A4.5 4.5 0 0 1 9 12 M23 12 A4.5 4.5 0 0 1 23 21 A4.5 4.5 0 0 1 23 12"
        ></path>
      </svg>
    </a>
    <h1 class="mt2 mb0 baskerville i fw1 f1">Title</h1>
    <h2 class="mt2 mb0 f6 fw4 ttu tracked">Your amazing subtitle</h2>
    <nav class="bt bb tc mw7 center mt4">
      <a
        class="
          f6
          f5-l
          link
          bg-animate
          black-80
          hover-bg-lightest-blue
          dib
          pa3
          ph4-l
        "
        href="/"
        >Home</a
      >
      <a
        class="
          f6
          f5-l
          link
          bg-animate
          black-80
          hover-bg-light-green
          dib
          pa3
          ph4-l
        "
        href="/portfolio"
        >Portfolio</a
      >
      <a
        class="
          f6
          f5-l
          link
          bg-animate
          black-80
          hover-bg-light-blue
          dib
          pa3
          ph4-l
        "
        href="/shop"
        >Shop</a
      >
      <a
        class="
          f6
          f5-l
          link
          bg-animate
          black-80
          hover-bg-light-pink
          dib
          pa3
          ph4-l
        "
        href="/about"
        >About</a
      >
      <a
        class="
          f6
          f5-l
          link
          bg-animate
          black-80
          hover-bg-light-yellow
          dib
          pa3
          ph4-l
        "
        href="/contact"
        >Contact</a
      >
    </nav>
  </header>
</template>
<style scoped>
.ba {
  border-style: solid;
  border-width: 1px;
}

.bt {
  border-top-style: solid;
  border-top-width: 1px;
}

.bb {
  border-bottom-style: solid;
  border-bottom-width: 1px;
}

.b--black {
  border-color: #000;
}

.br-100 {
  border-radius: 100%;
}

.dib {
  display: inline-block;
}

.avenir {
  font-family: 'avenir next', avenir, sans-serif;
}

.baskerville {
  font-family: baskerville, serif;
}

.i {
  font-style: italic;
}

.fw1 {
  font-weight: 100;
}

.fw4 {
  font-weight: 400;
}

.h2 {
  height: 2rem;
}

.tracked {
  letter-spacing: 0.1em;
}

.link {
  text-decoration: none;
  transition: color 0.15s ease-in;
}

.link:link,
.link:visited {
  transition: color 0.15s ease-in;
}

.link:hover {
  transition: color 0.15s ease-in;
}

.link:active {
  transition: color 0.15s ease-in;
}

.link:focus {
  transition: color 0.15s ease-in;
  outline: 1px dotted currentColor;
}

.mw7 {
  max-width: 48rem;
}

.w2 {
  width: 2rem;
}

.black-80 {
  color: rgba(0, 0, 0, 0.8);
}

.white {
  color: #fff;
}

.bg-black-80 {
  background-color: rgba(0, 0, 0, 0.8);
}

.bg-white {
  background-color: #fff;
}

.hover-bg-light-yellow:hover {
  background-color: #fbf1a9;
}

.hover-bg-light-yellow:focus {
  background-color: #fbf1a9;
}

.hover-bg-light-pink:hover {
  background-color: #ffa3d7;
}

.hover-bg-light-pink:focus {
  background-color: #ffa3d7;
}

.hover-bg-light-green:hover {
  background-color: #9eebcf;
}

.hover-bg-light-green:focus {
  background-color: #9eebcf;
}

.hover-bg-light-blue:hover {
  background-color: #76c4e2;
}

.hover-bg-light-blue:focus {
  background-color: #76c4e2;
}

.hover-bg-lightest-blue:hover {
  background-color: #cdecff;
}

.hover-bg-lightest-blue:focus {
  background-color: #cdecff;
}

.pa3 {
  padding: 1rem;
}

.pv4 {
  padding-top: 2rem;
  padding-bottom: 2rem;
}

.mb0 {
  margin-bottom: 0;
}

.mt2 {
  margin-top: 0.5rem;
}

.mt4 {
  margin-top: 2rem;
}

.tc {
  text-align: center;
}

.ttu {
  text-transform: uppercase;
}

.f1 {
  font-size: 3rem;
}

.f6 {
  font-size: 0.875rem;
}

.center {
  margin-right: auto;
  margin-left: auto;
}

.bg-animate,
.bg-animate:hover,
.bg-animate:focus {
  transition: background-color 0.15s ease-in-out;
}

@media screen and (min-width: 60em) {
  .ph4-l {
    padding-left: 2rem;
    padding-right: 2rem;
  }

  .f5-l {
    font-size: 1rem;
  }
}
</style>
