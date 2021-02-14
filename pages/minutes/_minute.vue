<template>
  <div class="minutes">
    <h1>{{ page.title }}</h1>
    <nuxt-content :document="page" />
  </div>
</template>

<script>
export default {
    async asyncData ({ $content, params }) {
        const page = await $content("minutes", params.minute, "index").fetch()

        return {
            page
        }
    }
}
</script>
