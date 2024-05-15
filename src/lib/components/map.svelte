<script lang="ts">
	export let location = 'Dover Harbour Board';
	export let height = '500px';
	export let showSatellite = false;
	export let width = '100%';
	export let zoom = 9;

	const queryParams = new URLSearchParams({
		q: location,
		t: showSatellite ? 'k' : '',
		z: `${zoom}`,
		ie: 'UTF8',
		output: 'embed',
	});

	const url = `https://maps.google.com/maps?${queryParams.toString()}`;
</script>

<div class="my-5" style="width: {width}; height: {height};">
	<iframe
		class="is-block"
		id="mapcanvas"
		title="Map"
		height="100%"
		width="100%"
		frameborder="0"
		scrolling="no"
		marginheight="0"
		marginwidth="0"
		src={url}
	/>
</div>
