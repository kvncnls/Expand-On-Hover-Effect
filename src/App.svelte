<script>
	import FooterLink from './FooterLink.svelte';
	let linkedIn = "Straight to business? LFG!";
	let twitter = "Follow me on Twitter!";
	let dribbble = "Check out my latest designs!";
	let email = "Send me an email!";

</script>

<main>
	<footer>
		<FooterLink src="https://dribbble.com" linkName="Dribbble" content="{dribbble}"></FooterLink>
		<FooterLink src="https://twitter.com" linkName="Twitter" content="{twitter}"></FooterLink>
		<FooterLink src="https://linkedin.com" linkName="LinkedIn" content="{linkedIn}" ></FooterLink>
		<!-- <FooterLink src="#" linkName="Email" content="{email}" ></FooterLink> -->
	</footer>
</main>

<style lang="scss">
	@import url('https://fonts.googleapis.com/css2?family=Passion+One:wght@700&display=swap');

	main {
		background-color: orangered;
		display: flex;
		flex-wrap: wrap;
		align-items: center;
		justify-content: space-between;
		width: 100%;
		height: 100%;
		max-width: 1200px;
		padding: 1rem;
		@media (orientation: portrait) {
			flex-direction: column;
		}
		@media (min-width: 1024px) {
			flex-direction: row;
		}
		footer {
			background-color: orangered;
			display: flex;
			flex-wrap: wrap;
			flex-direction: column;
			align-items: center;
			justify-content: space-between;
			height: 380px;
			width: 100%;
			@media (min-width: 768px) {
				flex-direction: row;
			}
		}

	}
</style>