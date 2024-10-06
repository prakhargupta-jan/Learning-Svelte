<script lang='ts'>
    export let age: Number;
    export let name: String
    export let gender: "Male" | "Female"
    export let property: "Hot" | "Ugly" | "Fat" | "Skinny" | "Black" | "White" | "Brown" | "Petite" | "Tall" | "Knockers";
</script>

<p>{name} is {age} years old, and {gender === "Male" ? "He" : "She"} is {property}</p>