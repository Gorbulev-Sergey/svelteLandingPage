<script>
	import After from '$lib/components/After.svelte';
	import Before from './Before.svelte';

	/**
	 * @type {any[]}
	 */
	export let routes = [];
</script>

<Before>
	<nav
		class="position-fixed w-100 d-flex flex-column align-items-center justify-content-between bg-light bg-opacity-10 px-3 py-2">
		<a href="/" class="btn btn-light text-dark border-0 text-uppercase" style="background:rgba(243,218,11,.4)">
			<b>Наш продукт</b>
		</a>
	</nav>
	<nav
		class="position-fixed bottom-0 w-100 d-flex flex-column align-items-center justify-content-between bg-light bg-opacity-10 px-3 py-2">
		<div class="d-flex align-items-center gap-1">
			{#each routes as item}
				<a href="#{item.url}" class="btn btn-sm btn-light bg-light bg-opacity-50 border-0 text-dark">{item.text}</a>
			{/each}
		</div>
	</nav>
</Before>
<After>
	<nav class="position-fixed w-100 d-flex align-items-center justify-content-between bg-light bg-opacity-10 px-3 py-2">
		<a href="/" class="btn btn-light text-dark border-0 text-uppercase" style="background:rgba(243,218,11,.4)">
			<b>Наш продукт</b>
		</a>
		<div class="d-flex align-items-center gap-2">
			{#each routes as item}
				<a href="#{item.url}" class="btn btn-light bg-light bg-opacity-50 border-0 text-dark">{item.text}</a>
			{/each}
		</div>
	</nav>
</After>
