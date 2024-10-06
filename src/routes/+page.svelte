<script>
	const colors = ['red', 'orange', 'yellow', 'green', 'blue', 'indigo', 'violet'];
	let selected = colors[0];
</script>

<h1 style="color: {selected}">Hello world!</h1>

<div>
	{#each colors as color}
		<button on:click={() => (selected = color)} style="background: {color}" />
	{/each}
</div>
<style>
    div {
        display: flex;
        width: 100%;
        flex-wrap: wrap;
        justify-content: space-evenly;
    }
    button {
        width: 50px;
        height: 50px;
        border-radius: 50%;
        border: 0;
        margin: 10px;
        cursor: pointer;
    }

</style>
