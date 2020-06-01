<template>
  <nav class="nav-primary">
    <ul>
      <li>
        <a href="#intro" v-smooth-scroll>European Accessibility Act?</a>
      </li>
      <li>
        <a href="#scope" v-smooth-scroll>Scope</a>
      </li>
      <li>
        <a href="#exceptions" v-smooth-scroll>Exceptions</a>
      </li>
      <li>
        <a href="#things-unclear" v-smooth-scroll>What is yet unclear?</a>
      </li>
      <li>
        <a href="#timeline" v-smooth-scroll>Timeline</a>
      </li>
      <li>
        <a href="#links" v-smooth-scroll>Links</a>
      </li>
    </ul>
  </nav>
</template>

<style>
  .nav-primary {
    position: fixed;
    left: 0;
    right: 0;
    background: #fff;
    width: 100%;
    top: 0;
    margin-top: 0;
    z-index: 1;
  }

  .nav-primary a {
    color: #0f0d34;
    text-decoration: none;
  }

  .nav-primary a:focus,
  .nav-primary a:hover {
    text-decoration: underline;
  }

  .nav-primary ul {
    max-width: 64rem;
    padding-left: 2rem;
    padding-right: 2rem;
    margin: auto;
    display: flex;
    justify-content: space-between;
  }

  .nav-primary li {
    padding: .5rem 0 .75rem;
  }

  @media (max-width: 600px) {
    html {
      font-size: 14px;
    }
  }

  @media screen and (max-width: 700px) {

    .nav-primary {
      position: relative;
      padding: .5rem 0 .75rem;
    }

    .nav-primary ul {
      flex-direction: column;
      margin-bottom: -1rem
    }

    .nav-primary li {
      padding-bottom: .5rem;
    }

  }
</style>
