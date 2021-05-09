<script>

</script>

<main>
	<a class="box box1" target="_blank" rel="noopener" href="https://dribbble.com">
		<h4>DRIBBLE</h4>
	</a>
	<a class="box box2" target="_blank" rel="noopener" href="https://linkedin.com">
		<h4>LINKEDIN</h4>
	</a>
	<a class="box box3" target="_blank" rel="noopener" href="https://twitter.com">
		<h4>TWITTER</h4>
	</a>
</main>

<style lang="scss">
	main {
		display: flex;
		flex-wrap: wrap;
		align-items: center;
		justify-content: space-between;
		@media (orientation: portrait) {
			flex-direction: column;
		}
		@media (min-width: 1024px) {
			flex-direction: row;
		}
		.box {
			background-color: orangered;
			padding: 2.5rem;
			color: white;
			display: flex;
			width: 100%;
			flex-grow: 1;
			flex-shrink: 1;
			flex-basis: 0;
			h4 {
				text-transform: uppercase;
			}
		}
	}
</style>