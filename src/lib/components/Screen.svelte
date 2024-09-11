<div class="screen">
	<slot />
</div>

<style>
	.screen {
		background-color: mediumturquoise;
		background-image: radial-gradient(rgba(51, 51, 51, 0.75), black 120%);
		width: 100vw;
		height: 100vh;
		text-shadow: 0 0 5px #c8c8c8;
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
