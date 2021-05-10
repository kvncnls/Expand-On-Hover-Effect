<script>
	import FooterLink from './FooterLink.svelte';

</script>

<main>
	<footer>
		<FooterLink src="https://dribble.com" linkName="Dribble"></FooterLink>
		<FooterLink src="https://twitter.com" linkName="Twitter"></FooterLink>
		<FooterLink src="https://linkedin.com" linkName="LinkedIn"></FooterLink>
	</footer>
</main>

<style lang="scss">
	@import url('https://fonts.googleapis.com/css2?family=Passion+One:wght@700&display=swap');

	main {
		background-color: rgb(36, 36, 36);
		display: flex;
		flex-wrap: wrap;
		align-items: center;
		justify-content: space-between;
		height: 100%;
		padding: 1rem;
		@media (orientation: portrait) {
			flex-direction: column;
		}
		@media (min-width: 1024px) {
			flex-direction: row;
		}
		footer {
			background-color: rgb(36, 36, 36);
			display: flex;
			flex-wrap: wrap;
			align-items: center;
			justify-content: space-between;
			height: 380px;
			width: 100%;
			@media (orientation: portrait) {
				flex-direction: column;
			}
			@media (min-width: 1024px) {
				flex-direction: row;
			}
		}

	}
</style>