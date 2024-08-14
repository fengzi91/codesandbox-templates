<script>
  let count = 0
  const increment = () => {
    count += 1
  }
</script>

<button on:click={increment} class="border border-blue-500 px-2 py-1 rounded-md bg-blue-500 hover:bg-blue-600 text-white">
  count is {count}
</button>
