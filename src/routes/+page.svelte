<script>
    let count = 0;
    const increment = () => count++;
    $: if (count >= 10) {
        alert('count is high');
        count = 0;
    }

</script>
<button on:click={increment}>{count} {count > 1 ? 'time' : 'times'}</button>
