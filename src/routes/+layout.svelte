<script>
	import Navbar from '$lib/components/navbar.svelte';
	import Footer from '$lib/components/footer.svelte';

	import '../app.scss';
</script>

<Navbar />

<div class="is-flex-grow-1">
	<slot />
</div>

<Footer />
