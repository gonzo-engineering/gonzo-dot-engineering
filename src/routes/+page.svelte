<svelte:head>
	<title>Gonzo Engineering</title>
	<meta name="description" content="Freak technology." />
</svelte:head>

<main>
	<p>The web is decedent and depraved.</p>
	<p>
		Gonzo Engineering is a project devoted to building free, open source tools for the benefit of
		journalists, musicians, and other members of the freak kingdom.
	</p>
	<p>Ventures so far:</p>
	<ul>
		<li>
			<a href="https://teeline.online">teeline.online</a>, an interactive learning site for Teeline
			shorthand
		</li>
		<li>
			<a href="https://github.com/gonzo-engineering/soli">Soli</a>, a 'just add water' toolkit for
			immersive musician websites
		</li>
	</ul>
	<p>
		Support the development of these tools and more by <a
			href="https://opencollective.com/gonzo-engineering">becoming a backer on Open Collective</a
		>. It all adds up.
	</p>
	<p>
		Want to collaborate? <a href="https://github.com/gonzo-engineering/">Join me on GitHub</a>
		or
		<a href="mailto:frederik.obrien@gmail.com">get in touch</a>.
	</p>
</main>

<style>
	main {
		padding: 1em;
		/* text-transform: lowercase; */
		text-shadow: 0 0 5px #c8c8c8;
	}
	a {
		font-weight: bold;
	}
	a:hover {
		opacity: 0.8;
	}
	ul {
		list-style-type: none;
		padding-left: 0;
		margin-bottom: 1em;
	}
	ul li::before {
		content: '>';
		margin-right: 0.5em;
	}
	@media (min-width: 768px) {
		main {
			position: absolute;
			top: 50%;
			left: 50%;
			transform: translate(-50%, -50%);
			max-width: 800px;
		}
	}
</style>
