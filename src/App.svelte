<script>
	export let name;
	import { Router, Route, Link } from "svelte-routing";
	import Home from "./Home.svelte";
	import SwingCompare from "./SwingCompare.svelte";
</script>

<Router>
	<nav>
		<Link to="/">Home</Link>
		<Link to="swing-compare">Swing Compare</Link>
	</nav>
	<Route path="/" component={Home} />
	<Route path="swing-compare" component={SwingCompare} />
</Router>



<main>
	<h1>Hell {name}!</h1>
	<p>
		Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
		how to build Svelte apps.
	</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
