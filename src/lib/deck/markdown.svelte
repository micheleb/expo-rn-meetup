<script lang="ts">
	export let name = "markdown.md";
	export let external = false;
</script>

{#if external}
	<section data-markdown={name}></section>
{:else}
	<section data-markdown>
		<div data-template>
			<slot />
		</div>
	</section>
{/if}
