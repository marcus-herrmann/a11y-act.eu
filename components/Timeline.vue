<template>
  <section class="section " id="timeline">
    <div class="section__inner">
      <h2>Timeline</h2>
      <ul class="timeline">
        <li>
          <div class="direction-r">
            <div class="flag-wrapper">
              <time datetime="2016-12-22" class="flag">December 22, 2016</time>
            </div>
            <div class="desc">
              Directive 2016/2102 comes into effect
            </div>
          </div>
        </li>
        <li>
          <div class="direction-l">
            <div class="flag-wrapper">
              <time datetime="2017-06-12" class="flag">June 12, 2017</time>
            </div>
            <div class="desc">
              Member states of the <abbr title="European Union">EU</abbr> are conferred power to adopt national law so as to make reference to a more recent version of that technical requirements.
            </div>
          </div>
        </li>
        <li>
          <div class="direction-r">
            <div class="flag-wrapper">
              <time datetime="2018-09-23" class="flag">September 23, 2018</time>
            </div>
            <div class="desc">
              All member states must have implementation laws based on directive 2102 in place. National infrastructure
              for supervision of compliance with Directive 2102 must be established. Office files published by public
              sector bodies after this date must be accessible. New websites of public sector bodies must be accessible.
            </div>
          </div>
        </li>
        <li>
          <div class="direction-l">
            <div class="flag-wrapper">
              <time datetime="2018-12-23" class="flag">December 23, 2018</time>
            </div>
            <div class="desc">
              Model accessibility statement will be published, technical requirements will be finalized. Standardized
              methodology of supervision and modalities of reporting from national level to the European Commission will
              be finalized.
            </div>
          </div>
        </li>
        <li>
          <div class="direction-r">
            <div class="flag-wrapper">
              <time datetime="2019-09-23" class="flag">September 23, 2019</time>
            </div>
            <div class="desc">
              Non public intranets and extranets must be accessible
            </div>
          </div>
        </li>
        <li>
          <div class="direction-l">
            <div class="flag-wrapper">
              <time datetime="2020-09-23" class="flag">September 23, 2020</time>
            </div>
            <div class="desc">
              Recorded time based media must be accessible. "Legacy" websites that have been published before September
              23, 2018 must be accessible.
            </div>
          </div>
        </li>
        <li>
          <div class="direction-r">
            <div class="flag-wrapper">
              <time datetime="2021-06-23" class="flag">June 23, 2021</time>
            </div>
            <div class="desc">Mobile apps of public sector bodies must be accessible</div>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<style>
  .timeline {
    position: relative;
    width: 660px;
    margin: 20px auto 0;
    padding: 1em 0;
    list-style-type: none;
  }

  .timeline:before {
    position: absolute;
    left: 50%;
    top: 0;
    content: " ";
    display: block;
    width: 6px;
    height: 100%;
    margin-left: -3px;
    background: #d9dd77;
    background: -moz-linear-gradient(
      top,
      rgba(80, 80, 80, 0) 0%,
      #d9dd77 8%,
      #d9dd77 92%,
      rgba(80, 80, 80, 0) 100%
    );
    background: -webkit-gradient(
      linear,
      left top,
      left bottom,
      color-stop(0%, rgba(30, 87, 153, 1)),
      color-stop(100%, rgba(125, 185, 232, 1))
    );
    background: -webkit-linear-gradient(
      top,
      rgba(80, 80, 80, 0) 0%,
      #d9dd77 8%,
      #d9dd77 92%,
      rgba(80, 80, 80, 0) 100%
    );
    background: -o-linear-gradient(
      top,
      rgba(80, 80, 80, 0) 0%,
      #d9dd77 8%,
      #d9dd77 92%,
      rgba(80, 80, 80, 0) 100%
    );
    background: -ms-linear-gradient(
      top,
      rgba(80, 80, 80, 0) 0%,
      #d9dd77 8%,
      #d9dd77 92%,
      rgba(80, 80, 80, 0) 100%
    );
    background: linear-gradient(
      to bottom,
      rgba(80, 80, 80, 0) 0%,
      #d9dd77 8%,
      #d9dd77 92%,
      rgba(80, 80, 80, 0) 100%
    );
    z-index: 5;
  }

  .timeline li {
    padding: 1em 0;
  }

  .timeline li:after {
    content: "";
    display: block;
    height: 0;
    clear: both;
    visibility: hidden;
  }

  .direction-l {
    position: relative;
    width: 300px;
    float: left;
    text-align: right;
  }

  .direction-r {
    position: relative;
    width: 300px;
    float: right;
  }

  .flag-wrapper {
    position: relative;
    display: inline-block;
    text-align: center;
  }

  .flag {
    position: relative;
    display: inline;
    background: rgb(248, 248, 248);
    padding: 6px 10px;
    border-radius: 5px;
    font-weight: 600;
    text-align: left;
    color: #0f0d34;
  }

  .direction-l .flag {
    -webkit-box-shadow: -1px 1px 1px rgba(0, 0, 0, 0.15),
    0 0 1px rgba(0, 0, 0, 0.15);
    -moz-box-shadow: -1px 1px 1px rgba(0, 0, 0, 0.15), 0 0 1px rgba(0, 0, 0, 0.15);
    box-shadow: -1px 1px 1px rgba(0, 0, 0, 0.15), 0 0 1px rgba(0, 0, 0, 0.15);
  }

  .direction-r .flag {
    -webkit-box-shadow: 1px 1px 1px rgba(0, 0, 0, 0.15),
    0 0 1px rgba(0, 0, 0, 0.15);
    -moz-box-shadow: 1px 1px 1px rgba(0, 0, 0, 0.15), 0 0 1px rgba(0, 0, 0, 0.15);
    box-shadow: 1px 1px 1px rgba(0, 0, 0, 0.15), 0 0 1px rgba(0, 0, 0, 0.15);
  }

  .direction-l .flag:before,
  .direction-r .flag:before {
    position: absolute;
    top: 50%;
    right: -39px;
    content: " ";
    display: block;
    width: 18px;
    height: 18px;
    margin-top: -7px;
    background: #0f0d34;
    border-radius: 10px;
    border: 6px solid #d9dd77;
    z-index: 10;
  }

  .direction-r .flag:before {
    left: -39px;
  }

  .direction-l .flag:after {
    content: "";
    position: absolute;
    left: 100%;
    top: 50%;
    height: 0;
    width: 0;
    margin-top: -8px;
    border: solid transparent;
    border-left-color: rgb(248, 248, 248);
    border-width: 8px;
    pointer-events: none;
  }

  .direction-r .flag:after {
    content: "";
    position: absolute;
    right: 100%;
    top: 50%;
    height: 0;
    width: 0;
    margin-top: -8px;
    border: solid transparent;
    border-right-color: rgb(248, 248, 248);
    border-width: 8px;
    pointer-events: none;
  }

  .direction-r .desc {
    margin: 1em 0 0 0;
  }

  .desc {
    margin-top: 1rem;
  }

  .desc ul,
  .desc li {
    margin-top: 0;
    padding-top: 0;
    padding-bottom: 0.5rem;
  }

  @media screen and (max-width: 700px) {
    .timeline {
      width: 100%;
      padding: 4em 0 1em 0;
    }

    .timeline li {
      padding: 2em 0;
    }

    .direction-l,
    .direction-r {
      float: none;
      width: 100%;

      text-align: center;
    }

    .flag-wrapper {
      text-align: center;
    }

    .flag {
      background: rgb(255, 255, 255);
      z-index: 15;
    }

    .direction-l .flag:before,
    .direction-r .flag:before {
      position: absolute;
      top: -22px;
      left: 50%;
      content: " ";
      display: block;
      width: 12px;
      height: 12px;
      margin-left: -6px;
      background: #0f0d34;
      border-radius: 10px;
      border: 4px solid #fff;
      z-index: 10;
    }

    .direction-l .flag:after,
    .direction-r .flag:after {
      content: "";
      position: absolute;
      left: 50%;
      top: -8px;
      height: 0;
      width: 0;
      margin-left: -8px;
      border: 8px solid transparent;
      border-bottom-color: rgb(255, 255, 255);
      pointer-events: none;
    }

    .desc {
      position: relative;
      margin: 1em 0 0 0;
      padding: 1em;
      background: rgba(27, 40, 90, .95);
      border-radius: 10px;
      z-index: 15;
    }

    .direction-l .desc,
    .direction-r .desc {
      position: relative;
      margin: 1em 1em 0 1em;
      padding: 1em;
      z-index: 15;
    }
  }
</style>
