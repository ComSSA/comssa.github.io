<template>
  <b-container fluid class="profile">
    <b-row>
      <b-col>
        <v-lazy-image
          class="rounded-corner portrait"
          :src="image"
        />
      </b-col>
    </b-row>
    <b-row id="name">
      <b-col>
        {{ name }}
      </b-col>
    </b-row>
    <b-row id="title">
      <b-col>
        {{ title }}
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
    name: "CloudProfile",
    props: {
        name: {
            type: String,
            required: true
        },
        title: {
            type: String,
            default: ""
        }
    },
    computed: {
        image () {
            return "https://cdn.comssa.org.au/committee-photos-2025/" + this.name.replace(/\s+/g, "%20") + ".JPG"
        }
    }
}
</script>
