<script>
  import { onMount } from 'svelte'
  let firstName = '', lastName = '';
  onMount(() => {
    const params = new URLSearchParams(window.location.search);
    firstName = params.get('firstName') || 'John';
    lastName = params.get('lastName') || 'Doe';
  })
</script>

<h1>
  Hi, I'm {firstName} {lastName}
</h1>
<p>I'm a fullstack developer</p>