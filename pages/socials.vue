<template>
  <b-container fluid>
    <h1 class="mt-3">
      Socials
    </h1>
    <b-row align-h="start" class="mt-5">
      <b-col md="auto">
        <iframe
          id="discord_embed"
          src="https://discord.com/widget?id=673182254930984980&theme=dark"
          allowtransparency="true"
          frameborder="0"
          sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"
        />
      </b-col>
      <b-col>
        <div
          class="fb-page"
          data-href="https://www.facebook.com/ComSSACurtin"
          data-tabs="timeline"
          data-width=""
          data-height="500"
          data-small-header="true"
          data-adapt-container-width="true"
          data-hide-cover="true"
          data-show-facepile="true"
        >
          Facebook timeline (may be blocked by your ad/tracker-blocker - fair enough)
          <blockquote
            cite="https://www.facebook.com/ComSSACurtin"
            class="fb-xfbml-parse-ignore"
          >
            <a href="https://www.facebook.com/ComSSACurtin" />
          </blockquote>
        </div>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
    head: {
        title: "Socials"
    },

    mounted () { // Facebook embeds do not appear on component mount, for some reason the included script has to be reloaded
        this.$loadScript(
            "https://connect.facebook.net/en_GB/sdk.js#xfbml=1&version=v9.0"
        ).then(() => {
            this.$nextTick(() => {
                window.FB.XFBML.parse()
            })
        }).catch(() => {
        })
    }
}
</script>
