<template>
  <section>
    <header>
      <h3>Area 51</h3>
      <p>"External" area index located in node_modules</p>
    </header>
    <output>
      <PageInfo />
    </output>
    <section>
      <h3>{{ greeting }}</h3>
      <p class="small dim" style="margin-top: 1rem">I have come from <a href="https://github.com/davestewart/area-51" target="_blank">Planet GitHub</a> !</p>
    </section>
  </section>
</template>

<script>
export default {
  computed: {
    greeting () {
      const { greeting, name } = this.$store.state.fiftyOne
      return `${greeting}, ${name}! 👽`
    }
  },

  mounted () {
    this.$store.dispatch('app/setSplash', require('../../docs/area-51.png'))
  },

  destroyed () {
    this.$store.dispatch('app/setSplash')
  }
}
</script>
