<script lang="ts">
	export let id: string | null = null;
	export let lines: string | boolean | null = null;
	export let noescape = false;
</script>

<pre data-id={id || null}>
  <code data-line-numbers={lines || null} data-noescape={noescape} data-trim><slot /></code>
</pre>
