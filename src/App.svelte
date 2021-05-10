<script>
	import FooterLink from './FooterLink.svelte';

</script>

<main>
	<footer>
		<FooterLink src="https://dribble.com" linkName="Dribble" content="Check out my latest web designs!"></FooterLink>
		<FooterLink src="https://twitter.com" linkName="Twitter" content="Follow me on Twitter!"></FooterLink>
		<FooterLink src="https://linkedin.com" linkName="LinkedIn" content="All business, eh? Come over to LinkedIn!"></FooterLink>
	</footer>
</main>

<style lang="scss">
	@import url('https://fonts.googleapis.com/css2?family=Passion+One:wght@700&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;300;500;700;900&display=swap');
	main {
		background-color: rgb(20, 20, 20);
		display: flex;
		flex-wrap: wrap;
		align-items: center;
		justify-content: space-between;
		height: 100%;
		padding: 1rem;
		max-width: 1200px;
		@media (orientation: portrait) {
			flex-direction: column;
		}
		@media (min-width: 1024px) {
			flex-direction: row;
		}
		footer {
			background-color: rgb(20, 20, 20);
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