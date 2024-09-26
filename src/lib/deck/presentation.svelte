<script lang="ts">
	import Code from './code.svelte';
	import Markdown from './markdown.svelte';
	import Notes from './notes.svelte';
	import Slide from './slide.svelte';
</script>

<Slide animate>
	<p>First</p>
</Slide>

<Slide animate>
	<p>First</p>
	<p>Slide!</p>
</Slide>

<Slide animate>
	<p>First</p>
	<p>Slide!</p>
	<p>With <a href="https://github.com" target="_blank">links</a>!</p>
</Slide>

<Slide animate>
	<p>First</p>
	<p>Slide!</p>
	<p>With <a href="https://github.com" target="_blank">links</a>!</p>
	<p>Press <span class="font-mono bg-slate-200 text-indigo-900 px-2 py-1">s</span> for Speaker Notes</p>
	<Notes>Here are some speaker notes, too</Notes>
</Slide>

<Markdown>
	{`
# Markdown Slide
- This is another slide
- and it's written in Markdown!

---

# Another Markdown Slide
- You can create multiple slides at once!
	`}
</Markdown>

<Markdown external name="external-example.md" />

<Slide animate>
	<Code id="code" lines="|2">
		{`
		const myFunction = (message: string) => {
			console.log(message);
		}
		`}
	</Code>
</Slide>

<Slide animate>
	<Code id="code" lines="|3">
		{`
		const myFunction = (message: string) => {
			console.log(message);
			console.log("done!");
		}
		`}
	</Code>
</Slide>