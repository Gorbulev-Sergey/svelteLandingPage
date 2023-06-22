<script>
	import Nav from '$lib/components/Nav.svelte';
	let routes = [
		{ text: 'Продукт', url: 'a1' },
		{ text: 'Цвет', url: 'a2' },
		{ text: 'Форма', url: 'a3' },
		{ text: 'Оформить', url: 'a4' }
	];
</script>

<Nav {routes} />
<slot />
