<script lang="ts">
  let counter = $state(0)

  function inc() {
    ++counter
  }

  function dec() {
    counter -= 1
  }
</script>

<main>
  <h1>Counter: {counter}</h1>
  <div class="buttons">
    <button onclick={inc}>+</button>
    <button onclick={dec}>-</button>
  </div>
</main>

<style>
  button {
    font-size: 40px;
  }

  .buttons {
    display: flex;
    flex-direction: row;
    gap: 100px;
  }

  main {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
</style>
