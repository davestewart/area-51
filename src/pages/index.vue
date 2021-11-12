<template>
  <section>
    <h3>Area 51</h3>
    <output>
      <pre>node_modules/area-51/src/pages/index</pre>
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
