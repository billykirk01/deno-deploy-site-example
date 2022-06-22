<script>
    import { onMount } from "svelte";

    onMount(async () => {
        fetch("/api/time")
            .then((response) => response.json())
            .then((data) => {
                console.log(data);
            })
            .catch((error) => {
                console.log(error);
            });
    });
</script>

<h1>Hello from Svelte and Deno!</h1>
