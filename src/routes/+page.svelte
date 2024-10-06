<script lang='ts'>
    let count = 0;
    const increment = () => count++;
</script>
<button on:click={increment}>
    Clicked {count}
</button>

{#if count > 10}
    <p>{count} is greater than 10.</p>
{/if}