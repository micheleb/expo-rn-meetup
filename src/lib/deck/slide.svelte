<script lang="ts">
	export let id: string | null = null;
	export let animate = false;
	export let backgroundImage: string | null = null;
	export let restart = false;
</script>

<section
	data-auto-animate={animate || null}
	data-auto-animate-id={id}
	data-auto-animate-restart={restart || null}
	data-background-image={backgroundImage || null}
>
	<slot />
</section>
