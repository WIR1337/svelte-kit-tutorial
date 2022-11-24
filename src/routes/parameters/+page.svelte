<script>
import Message from "./Message.svelte";

let a = {
    name: 'Alexander',
    wish: 'Nice Day'
}

</script>

<a href="/">Home</a>
<!-- Spread for parameters -->
<Message {...a}></Message>

