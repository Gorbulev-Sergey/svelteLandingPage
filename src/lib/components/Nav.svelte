<script>
	/**
	 * @type {any[]}
	 */
	export let routes = [];
</script>

<nav class="position-fixed w-100 d-flex align-items-center justify-content-between bg-light bg-opacity-10 px-3 py-2">
	<a href="/" class="btn btn-light text-dark border-0 text-uppercase" style="background:rgba(243,218,11,.4)">
		<b>Наш продукт</b>
	</a>
	<div class="d-flex align-items-center">
		{#each routes as item}
			<a href="#{item.url}" class="btn btn-light bg-light bg-opacity-50 border-0 text-dark ms-2">{item.text}</a>
		{/each}
	</div>
</nav>
