<script>
	let content = 'Hello World!'
	let src = 'https://svelte.dev/svelte-logo-horizontal.svg'
</script>

<h1>{content}</h1>

<img alt='logo' {src}>
<img alt='logo' src="{src}">

<style>
	
</style>