<script>
	import schema from '$lib/data/schema-org.json';
</script>

<svelte:head>
	<title>Gonzo Engineering</title>
	<meta
		name="description"
		content="Building free, open source tools for journalists, musicians, and other members of the freak kingdom."
	/>
</svelte:head>

<main>
	<h2>The Web Is Decadent and Depraved</h2>
	<p>
		Gonzo Engineering is devoted to building free, open source tools for the benefit of journalists,
		musicians, and other members of the freak kingdom.
	</p>
	<p>Ventures so far:</p>
	<ul>
		<li>
			<a href="https://teeline.online">teeline.online</a> - an interactive learning site for Teeline
			shorthand
		</li>
		<li>
			<a href="https://soli.network">Soli</a> - music streaming with direct, transparent remuneration
			for artists
		</li>
		<li>
			<a href="https://github.com/gonzo-engineering/skene">Skene</a> - a 'just add water' template for
			musician websites
		</li>
		<li>
			<a href="https://github.com/gonzo-engineering/dummy">Dummy</a> - a miniature tech stack for shoestring
			news publishing
		</li>
	</ul>
	<p>
		Support the development of these projects and more by <a
			href="https://ko-fi.com/frederickobrien">buying me a coffee</a
		>
		or
		<a href="https://opencollective.com/gonzo-engineering">becoming a backer on Open Collective</a>.
		It all adds up.
	</p>
	<p>
		Want to collaborate? <a href="mailto:frederik.obrien@gmail.com">Get in touch</a> or
		<a href="https://github.com/gonzo-engineering/">get involved</a>.
	</p>
	<p>In solidarity,</p>
	<p>Frederick<span class="flashing-underscore">_</span></p>
</main>

{@html `<script type="application/ld+json">${JSON.stringify(schema)}</script>`}

<style>
	main {
		padding: 1em;
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
	.flashing-underscore {
		animation: flashing-underscore 1.5s infinite;
	}
	@keyframes flashing-underscore {
		0% {
			opacity: 1;
		}
		50% {
			opacity: 0;
		}
		100% {
			opacity: 1;
		}
	}
</style>
