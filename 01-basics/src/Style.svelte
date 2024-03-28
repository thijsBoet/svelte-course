<h1>My First Svelte component</h1>

<p class="links">Hello World</p>
<div>
	<a href="https://www.youtube.com/c/lihautan">Link to my youtube Channel</a>
</div>

<Component />

<style>
	:global(h1) {
		color: rebeccapurple;
		animation: zoom 5s;
	}
	:global(p) {
		font-size: 44px;
	}
	.links {
		text-align: right;
	}
	@keyframes -global-zoom {
		0%, 100% { transform: scale(3)}
		50% {transform: scale(0.5)}
	}
</style>

<script>
	const name ="Matthijs Boet"
	import Component from './Component.svelte'
</script>