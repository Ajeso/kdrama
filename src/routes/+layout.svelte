<script context="module">
	import Header from './Components/Header.svelte';
	import { siteName } from './+page.server.js';
	let headerData = {
		siteName: siteName,
		navLinks: [{ text: 'dramacool.pa', url: 'https://dramacool.pa' }]
	};
</script>

<div class="container bg-sky-300 p-7">
	<Header {headerData} />
	<main>
		<slot />
	</main>
</div>
