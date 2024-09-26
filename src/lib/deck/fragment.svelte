<script lang="ts">
	export let animation:
		| 'fade-out'
		| 'fade-up'
		| 'fade-down'
		| 'fade-left'
		| 'fade-right'
		| 'fade-in-then-out'
		| 'current-visible'
		| 'fade-in-then-semi-out'
		| 'grow'
		| 'semi-fade-out'
		| 'shrink'
		| 'strike'
		| 'highlight-red'
		| 'highlight-green'
		| 'highlight-blue'
		| 'highlight-current-red'
		| 'highlight-current-green'
		| 'highlight-current-blue'
		| null = null;
	export let inline = false;
</script>

<p class="fragment {animation || null} {inline ? "inline" : null}">
	<slot />
</p>
