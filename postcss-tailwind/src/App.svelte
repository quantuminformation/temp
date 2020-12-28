<script>
  const world = 'postcss'; // edit world and save to see hmr update
</script>

<style>
  h1 {
    color: orangered; /* change color an save to see hmr update */
    /* you can also use css nesting
    & .world {
      font-size: 2rem;
    }
    */
  }
  .world {
    @apply text-green-500 italic; /*  here's some tailwind apply */
  }
</style>

<h1 class="border border-current rounded p-4 m-4">
  <!-- tailwind classes in svelte template -->
  Hello
  <span class="world">{world}</span>
  <article class="text-sm sm:text-base">

    <textarea
      autofocus
      value="test"
      placeholder="Chat away.. Press ENTER or RETURN on your phone to send. Data will be deleted soon as still in development." />

    <span id="sendInstruction">Press enter to send</span>
    <p />
  </article>
</h1>
