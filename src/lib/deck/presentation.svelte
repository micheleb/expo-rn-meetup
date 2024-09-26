<script lang="ts">
	import Code from './code.svelte';
	import Markdown from './markdown.svelte';
	import Notes from './notes.svelte';
	import Slide from './slide.svelte';
</script>

<Slide backgroundImage="title-bg.jpg">
	<h1>Things that ChatGPT won't tell you about Expo</h1>
</Slide>

<Slide>
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

<Slide>
	<Slide animate>
    <Code id="code" lines>
        {`
{
  "cli": {
    "version": ">= 4.1.2",
    "appVersionSource": "remote"
  },
  "build": {
    "development": {
    },
    "simulator": {
    },
    "preview": {
    },
    "beta": {
    },
    "production": {
      "extends": "beta"
    }
  },
  "submit": {
    "beta": {},
    "production": {}
  }
}
    `}
    </Code>
	</Slide>

	<Slide animate>
    <Code id="code" lines>
        {`
{
  "cli": { /* ... */ },
  "build": {
    "development": {
      "developmentClient": true,
      "distribution": "internal",
      "channel": "development",
      "autoIncrement": true
    },
    "simulator": {
      "developmentClient": true,
      "distribution": "internal",
      "channel": "development",
      "autoIncrement": true,
      "ios": {
        "simulator": true
      }
    },
    "preview": {
      "distribution": "internal",
      "env": {
        "APP_VARIANT": "production"
      },
      "channel": "preview",
      "android": {
        "buildType": "apk"
      },
      "autoIncrement": true
    },
    "beta": {
      "env": {
        "APP_VARIANT": "production"
      },
      "channel": "production",
      "autoIncrement": true
    },
    "production": {
      "extends": "beta"
    }
  },
  "submit": {
    "beta": {},
    "production": {}
  }
}
    `}
    </Code>
	</Slide>

	<Slide animate>
    <Code id="code" lines="5">
        {`
{
  "cli": { /* ... */ },
  "build": {
    "development": {
      "developmentClient": true,
      "distribution": "internal",
      "channel": "development",
      "autoIncrement": true
    },
    "simulator": {
      "developmentClient": true,
      "distribution": "internal",
      "channel": "development",
      "autoIncrement": true,
      "ios": {
        "simulator": true
      }
    },
    "preview": {
      "distribution": "internal",
      "env": {
        "APP_VARIANT": "production"
      },
      "channel": "preview",
      "android": {
        "buildType": "apk"
      },
      "autoIncrement": true
    },
    "beta": {
      "env": {
        "APP_VARIANT": "production"
      },
      "channel": "production",
      "autoIncrement": true
    },
    "production": {
      "extends": "beta"
    }
  },
  "submit": {
    "beta": {},
    "production": {}
  }
}
    `}
    </Code>
	</Slide>

	<Slide animate>
    <Code id="code" lines="5,6">
        {`
{
  "cli": { /* ... */ },
  "build": {
    "development": {
      "developmentClient": true,
      "distribution": "internal",
      "channel": "development",
      "autoIncrement": true
    },
    "simulator": {
      "developmentClient": true,
      "distribution": "internal",
      "channel": "development",
      "autoIncrement": true,
      "ios": {
        "simulator": true
      }
    },
    "preview": {
      "distribution": "internal",
      "env": {
        "APP_VARIANT": "production"
      },
      "channel": "preview",
      "android": {
        "buildType": "apk"
      },
      "autoIncrement": true
    },
    "beta": {
      "env": {
        "APP_VARIANT": "production"
      },
      "channel": "production",
      "autoIncrement": true
    },
    "production": {
      "extends": "beta"
    }
  },
  "submit": {
    "beta": {},
    "production": {}
  }
}
    `}
    </Code>
    <Notes>Testing notes</Notes>
	</Slide>
</Slide>