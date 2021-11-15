<template>
  <section>
    <h3>Area 51</h3>
    <output>
      <PageInfo />
    </output>
    <section>
      <h3>{{ greeting }}</h3>
      <p class="small dim" style="margin-top: 1rem">I have travelled <a href="https://github.com/davestewart/area-51" target="_blank">far</a> !</p>
    </section>
  </section>
</template>

<script>
export default {
  computed: {
    greeting () {
      return 'Greetings, Earthling! 👽'
    }
  }
}
</script>
