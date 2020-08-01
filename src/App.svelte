<script>
  let visible = false;
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

  .box {
    margin-left: auto;
    margin-right: auto;
    width: 100px;
    height: 100px;
    background-color: blanchedalmond;
    opacity: 0.5;
    border: 1px solid #000;
  }

  .boxBlock {
    display: flex;
    margin-left: auto;
    margin-right: auto;
    margin-top: 50px;
    border: 1px solid #000;
    width: 300px;
    height: 100px;
  }

  .colorBox {
    width: 33%;
    height: 100%;
    border: 1px dashed #999;
  }

  .red {
    background-color: red;
  }

  .blue {
    background-color: blue;
  }

  .green {
    background-color: green;
  }
  .hide {
    display: none;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<main>

  <div class="box" />

  <div class="boxBlock ">
    <div class="colorBox red" on:click={(visible = !visible)} />
    <div class="colorBox blue" />
    <div class="colorBox green" />
  </div>
</main>
