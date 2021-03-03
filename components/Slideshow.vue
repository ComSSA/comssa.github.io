<template>
  <div>
    <b-carousel
      id="carousel"
      v-model="slide"
      :interval="4000"
      controls
      fade
      indicators
      img-width="1024"
      img-height="480"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <div v-for="image in images" :key="image">
        <b-carousel-slide :img-src="require(`~/assets/img/${rootDir}/${image}`)" />
      </div>
    </b-carousel>
  </div>
</template>

<script>
export default {
    props: {
        rootDir: {
            type: String,
            required: true
        },
        images: {
            type: Array,
            required: true
        }
    },
    data () {
        return {
            slide: 0,
            sliding: null
        }
    },
    methods: {
        onSlideStart (slide) {
            this.sliding = true
        },
        onSlideEnd (slide) {
            this.sliding = false
        }
    }
}
</script>
