<script>
	export let text = 'Текст';
	export let description = '';
	export let image = 'https://cdn1.ozone.ru/s3/multimedia-4/6128559676.jpg';
	export let color = '';
	export let textColor = '';
	export let reverse = false;
	export let anchor = '';
</script>

<div
	id={anchor}
	class="d-flex align-items-center justify-content-between {reverse ? 'flex-row-reverse' : ''} px-5 gap-3"
	style="min-height: 100vh; background:{color}">
	<div class="flex-grow-1 text-center">
		<h1 class="display-2" style="color:{textColor}">{text}</h1>
		<i class="text-muted display-6" style="font-size:1.3em">{description}</i>
	</div>
	<img class="rounded-5" style="max-height: 80vh; max-width:40vw" src={image} alt="" />
</div>
