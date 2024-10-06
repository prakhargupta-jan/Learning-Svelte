<script lang='ts'>
    import Nested from "../components/Nested.svelte";
    const person: {
        name: String,
        age: Number,
        gender: "Male" | "Female",
        property: "Hot" | "Ugly" | "Fat" | "Skinny" | "Black" | "White" | "Brown" | "Petite" | "Tall" | "Knockers";
    } = {
        name: "Ramesh",
        age: 22,
        gender: "Male",
        property: "Black",
    }
</script>
<Nested {...person} />