<script lang="ts">
  let inputValue: string = $state("");

  let counter: number = $state(0);

  $effect(() => {
    counter++;
  });
</script>

<link rel="style" href="../cssFiles/InputBox.css" />

<main>
  The input is {inputValue} <br />

  <input class="input1" bind:value={inputValue} type="string" /> <br />

  <p>
    {counter}
  </p>
</main>
