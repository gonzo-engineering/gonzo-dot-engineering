<script>
	export let backgroundColor = 'mediumturquoise';
</script>

<div class="screen" style="background-color: {backgroundColor}">
	<slot />
</div>

<style>
	.screen {
		position: relative;
		text-shadow: 0 0 5px #c8c8c8;
		background-image: radial-gradient(rgba(51, 51, 51, 0.75), black 120%);
		height: fit-content;
		min-height: 100vh;
	}
	.screen::after {
		content: '';
		position: absolute;
		pointer-events: none;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background: repeating-linear-gradient(
			0deg,
			rgba(0, 0, 0, 0.15),
			rgba(0, 0, 0, 0.15) 2px,
			transparent 2px,
			transparent 4px
		);
		pointer-events: none;
	}
</style>
