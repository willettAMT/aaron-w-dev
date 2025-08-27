<script lang="ts">
  let count: number = 0;
  const unclicked: string = "This is a counter!";
  const increment = () => {
    count += 1
  }
</script>

<button on:click={increment}>
  {count === 0 ? unclicked : `count is ${count}`}
</button>
