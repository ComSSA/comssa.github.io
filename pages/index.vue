<template>
  <b-container fluid>
    <b-row align-h="around" class="mb-5">
      <b-col>
        <h1 id="headline" class="display-3">
          <span>Com</span>puter <br>
          <span>S</span>cience <br>
          <span>S</span>tudents <br>
          <span>A</span>ssociation
        </h1>
        <div id="join-link">
          <NuxtLink to="/join">
            Register now
          </NuxtLink>
          <img id="arrow" src="~/assets/img/icon/forward-arr.svg">
        </div>
      </b-col>
      <b-col md="5" class="ml-5 mt-md-3">
        <div class="carousel-shadow">
          <Slideshow
            :link="false"
            css="front-page-carousel"
            root-dir="posters"
            :images="images"
          />
        </div>
      </b-col>
    </b-row>

    <b-row align-h="around">
      <b-col md="auto" class="mb-3">
        <v-lazy-image
          id="committee-photo"
          class="mt-xs-5 front-page-image rounded-corner"
          alt="Image of committee in front of ComSSA O-Day stall"
          :src="require('~/assets/img/commiteePhoto.jpg')"
        />
      </b-col>
      <b-col id="who-are-we">
        <h2>Who are we?</h2>

        <p>
          ComSSA is the club that supports computing, computer
          engineering, and networking students at Curtin University.
          <br><br>

          We also support non-computing students by providing events
          and services that give like minded individuals (anyone
          interested in programming or computing) a space to find
          support, socialise and communicate.<br><br>

          You do not need to be a computing student. Membership is
          open to everyone, even if you’re not a student! <br><br>

          Committee members can be found throughout the level 2 labs
          in building 314 or in the ComSSA common room (314.127).
          <NuxtLink to="/about">
            Not sure who we are?
          </NuxtLink>
          <br><br>

          ComSSA provides a wide
          <NuxtLink to="/events">
            range of events
          </NuxtLink>
          and services for its members, such as academic assistance,
          social events and industry orientated events. <br><br>

          ComSSA is affiliated with Curtin Student Guild which means
          if you are a Curtin student and have a voucher from the
          guild diary then membership is free.
        </p>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
const getPostersArray = () =>
    Array.from(
        require.context("~/assets/img/posters", true, /\.(jpg|png|svg)$/).keys()
    ).map(s => s.substr(2))

export default {
    data () {
        return { images: getPostersArray() }
    },

    head: {
        titleTemplate: "ComSSA"
    }
}
</script>
