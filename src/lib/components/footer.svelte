<script lang="ts">
	const startYear = 2024;
	const currentYear = new Date().getUTCFullYear();

	let copyrightYear = `${currentYear}`;
	if (currentYear > startYear) {
		copyrightYear = `${startYear} - ${copyrightYear}`;
	}
	const copyrightHolder = 'Bluebell Family History';

	// eslint-disable-next-line no-undef
	const description = __DESCRIPTION__;
</script>

<footer class="has-background-black-ter has-text-white py-6">
	<div class="container">
		<div class="columns has-text-centered-touch">
			<div class="column is-half">{description}</div>

			<div class="column is-half has-text-right-desktop">
				<a
					href="https://twitter.com/twitterUser"
					target="_blank"
					class="icon has-text-white"
				>
					<i class="mdi mdi-24px mdi-twitter"></i>
				</a>
			</div>
		</div>
		<hr class="has-background-grey-dark" />
		<p class="has-text-centered">
			&copy; {copyrightYear}
			{copyrightHolder}
		</p>
	</div>
</footer>
