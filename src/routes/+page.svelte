<script lang="ts">
    let numbers: number[] = [];
    let name = {
        firstName: "Vijay",
        lastName: "Sharma",
    }
    const addNumber = () => numbers = [...numbers, numbers.length + 1];
    const toggleName = () => name.lastName === "Sharma" ? name = {...name, lastName: "Gupta"} : name = {...name, lastName: "Sharma"};
     
</script>
<button on:click={toggleName}>Toggle Name: {name.firstName} {name.lastName}</button>
<button on:click={addNumber}>Add Number: {numbers.length}</button>