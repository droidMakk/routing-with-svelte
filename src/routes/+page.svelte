<script>
  import MessageContainer from "../components/MessageContainer.svelte";
  let welcomeMessage = 'Welcome to Svelte'
  let time = 0
</script>
<h1>{welcomeMessage}</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<MessageContainer message={`You've Clicked ${time} time${time > 1 ? 's' : ''}`} />
<button on:click={() => time++} >Click here.</button>
