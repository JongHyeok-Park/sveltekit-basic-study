<script lang="ts">
  let count = $state<number>(0);
</script>

<h1>about 페이지임</h1>
<button onclick={() => { count++ }}>
  clicks: {count}
</button>