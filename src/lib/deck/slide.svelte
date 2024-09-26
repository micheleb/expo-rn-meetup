<script lang="ts">
	export let id: string | null = null;
	export let animate = false;
	export let backgroundImage: string | null = null;
	export let restart = false;
	export let transition: 'slide' | 'fade' | null = null;
	export let uncounted = false;
</script>

<section
	data-auto-animate={animate || null}
	data-auto-animate-id={id}
	data-auto-animate-restart={restart || null}
	data-background-image={backgroundImage || null}
	data-transition={transition || null}
	data-visibility={uncounted ? 'uncounted' : null}
>
	<slot />
</section>
