<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;
</script>

<div class="content">
	<svelte:component this={data.content.Component} {data} />
</div>
