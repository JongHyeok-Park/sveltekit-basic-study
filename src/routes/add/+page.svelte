<script>
  let a = 0;
  let b = 0;
  let total = 0;

  const add = async () => {
    const response = await fetch('/api/add', {
      method: 'POST',
      body: JSON.stringify({ a, b }),
      headers: {
        'content-type': 'application/json'
      }
    });

    total = await response.json();
  }
</script>

<h1>Add</h1>
<input type="number" bind:value={a}> + <input type="number" bind:value={b}> = {total}
<button onclick={add}>calculate</button>