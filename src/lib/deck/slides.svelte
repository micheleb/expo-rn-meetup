<script lang="ts">
	import Reveal from 'reveal.js';
	import 'reveal.js/dist/reveal.css';
	import 'reveal.js/dist/theme/dracula.css';
	import Highlight from 'reveal.js/plugin/highlight/highlight';
	import './grayscale.css';
	import Markdown from 'reveal.js/plugin/markdown/markdown';
	import Notes from 'reveal.js/plugin/notes/notes';
	import { onMount } from 'svelte';

	import Presentation from './presentation.svelte';

	onMount(() => {
		const deck = new Reveal({
			autoAnimateDuration: 1,
			autoAnimateEasing: 'ease',
			controls: false,
			hash: true,
			plugins: [Highlight, Markdown, Notes],
			progress: true,
			transition: 'fade'
		});

		deck.initialize();

		if (import.meta.hot) {
			import.meta.hot.on('vite:afterUpdate', () => location.reload());
		}
	});
</script>

<div class="reveal">
	<div class="slides">
		<Presentation />
	</div>
</div>
