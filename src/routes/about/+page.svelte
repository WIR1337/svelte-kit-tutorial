<script lang="ts">
    import { onDestroy, onMount } from "svelte";

    let score: number = 0;

    let a = setInterval(() => {
            score += 1;
        }, 2000);
    onMount(() => a);
    onDestroy(() => {
        clearInterval(a)
        console.log("Timer was stoped");
    })
</script>

<a href="/">Home</a>
<h2>Запустился таймер , как только я покину страницу он отключится</h2>
<div>{score} this value increase every 2 seconds</div>
