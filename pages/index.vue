<template>
  <div class="wrapper">
    <header>
      <logo/>
      <navigation/>
    </header>
    <main class="container">
      <intro/>
      <scope/>
      <exceptions/>
      <unclear />
      <timeline/>
      <links/>
      <about/>
    </main>
    <site-footer/>
  </div>
</template>

<script>
  import Logo from "~/components/Logo.vue";
  import Navigation from "~/components/Navigation.vue";
  import Intro from "~/components/Intro.vue";
  import Scope from "~/components/Scope.vue";
  import Exceptions from "~/components/Exceptions.vue";
  import Timeline from "~/components/Timeline.vue";
  import Links from "~/components/Links.vue";
  import Unclear from "~/components/Unclear.vue";
  import About from "~/components/About.vue";
  import SiteFooter from "~/components/SiteFooter.vue";

  export default {
    components: {
      Logo,
      Navigation,
      Intro,
      Scope,
      Exceptions,
      Unclear,
      Timeline,
      Links,
      About,
      SiteFooter
    }
  };
</script>

<style>

  /* ibm-plex-sans-regular - latin */
  @font-face {
    font-family: 'IBM Plex Sans';
    font-style: normal;
    font-weight: 400;
    src: local('IBM Plex Sans'), local('IBMPlexSans'),
    url('/fonts/ibm-plex-sans-v2-latin-regular.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
    url('/fonts/ibm-plex-sans-v2-latin-regular.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
  }

  /* ibm-plex-sans-700 - latin */
  @font-face {
    font-family: 'IBM Plex Sans';
    font-style: normal;
    font-weight: 700;
    src: local('IBM Plex Sans Bold'), local('IBMPlexSans-Bold'),
    url('/fonts/ibm-plex-sans-v2-latin-700.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
    url('/fonts/ibm-plex-sans-v2-latin-700.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
  }

  html {
    background: #0f0d34 linear-gradient(to right top, #204885, #1e3870, #1b295b, #151b47, #0f0d34) fixed;
  }

  h2 {
    margin-bottom: 1em;
    text-align: center;
  }

  h3 {
    color: #d9dd77;
  }

  blockquote {
    font-style: italic;
    margin: 1rem;
  }

  blockquote:before {
    content: '» ';
  }

  blockquote:after {
    content: '«';
  }

  header {
    background: #fff;
    min-height: 5rem;
    position: relative;
    margin-bottom: 3rem;
  }

  header:after {
    content: '';
    position: absolute;
    left: 0;
    right: 0;
    top: 2rem;
    bottom: -2rem;
    background: #fff;
    z-index: -1;
    transform: skewY(-2deg);
  }

  .container {
    min-height: 100vh;
    margin: auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    line-height: 1.72;
    font-size: 1.1rem;
    color: #fff;
  }

  .section {
    margin-bottom: 2rem;
    transform: skewY(-2deg);
    display: flex;
    justify-content: center;
  }

  .section__inner {
    max-width: 64rem;
    padding-left: 2rem;
    padding-right: 2rem;
    transform: skewY(2deg);
    margin-top: 5rem;
    margin-bottom: 5rem;
    width: 100%;
  }

  .section--highlighted {
    background: rgba(255, 255, 255, .1);
  }

  ul,
  p {
    margin: 1rem 0;
  }

  ul,
  li {
    padding: 0;
    margin: 0;
    list-style: none;
  }

  ul.text-list {
    padding-left: 15px;
  }

  .text-list li {
    list-style-type: none;
    position: relative;
    margin-bottom: 0.75em;
  }

  .text-list li:before {
    content: '•';
    display: inline-block;
    position: absolute;
    left: -.8em;
    color: #d9dd77;
  }

  a {
    color: #fff;
    font-weight: bold;
    transition: color .25s;
  }

  a:hover,
  a:focus {
    color: #d9dd77;
  }

  @media screen and (max-width: 700px) {

    header {
      display: flex;
      flex-direction: row-reverse;
      margin-bottom: 1rem;
    }

    header::after {
      bottom: -.5rem;
    }

    h2 {
      margin-bottom: .5em;
    }

    .logo-icon {
      margin-top: 0;
      margin-bottom: 0;
    }

    .section {
      margin-bottom: 0;
      padding-bottom: 2rem;
    }

    .section__inner {
      margin: 3rem auto 0;
    }

    .container {
      padding-bottom: 4rem;
    }

  }

</style>
