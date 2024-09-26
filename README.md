# svelte-revealjs-slides-template

A template project to be cloned to create [reveal.js](https://revealjs.com) slides, using [SvelteKit](https://kit.svelte.dev).

This is based on [Create Beautiful Presentations With Svelte](https://www.youtube.com/watch?v=67lqa5kTQkA) by [Joy of Code](https://www.youtube.com/@JoyofCodeDev)

## Creating a project

Clone the repo, then run

```bash
pnpm i
```

## Developing

Once you've installed dependencies, start a development server:

```bash
pnpm dev --open
```

Omit the `--open` option if you don't want to launch a new browser.

The main presentation file is in [`presentation.svelte`](./src/lib/deck/presentation.svelte), start from there to edit your slides.

Refer to the [reveal.js docs](https://revealjs.com) for more documentation.

## Building

To create a production version of your slides:

```bash
pnpm build
```

You can preview the production build with `pnpm preview`.
