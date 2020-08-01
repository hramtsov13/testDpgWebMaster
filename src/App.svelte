<script>
  let name = "Svelte";
</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  :global(h1) {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  .playground {
    margin-left: auto;
    margin-right: auto;
    width: 100px;
    height: 100px;
    background-color: blanchedalmond;
    opacity: 0.5;
    border: 1px solid #000;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<main>
  <h1>{name}</h1>

  <div class="playground" />

</main>
