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
		<h2>Talking About</h2>
	</Slide>

	<Slide animate>
		<Notes>
			<ul>
				<li>How many have used Expo?</li>
				<li>How many in prod now?</li>
			</ul>
		</Notes>
		<h2>Talking About</h2>
		<p>Expo (duh)</p>
	</Slide>

	<Slide animate>
		<Notes>
			<ul>
				<li>Official Docs, GitHub issues, Discord</li>
				<li>ChatGPT! but it hallucinates and knowledge cutoff</li>
			</ul>
		</Notes>
		<h2>Talking About</h2>
		<p>Expo (duh)</p>
		<p>Where's the info?</p>
	</Slide>

	<Slide animate>
		<Notes>
			<ul>
				<li>Expo is pushed heavily, you might think it's a you problem</li>
			</ul>
		</Notes>
		<h2>Talking About</h2>
		<p>Expo (duh)</p>
		<p>Where's the info?</p>
		<p>It's not me, it's you</p>
	</Slide>

	<Slide animate>
		<Notes>
			<ul>
				<li>I might not know things</li>
				<li>QR Code with link at the end</li>
			</ul>
		</Notes>
		<h2>Talking About</h2>
		<p>Expo (duh)</p>
		<p>Where's the info?</p>
		<p>It's not me, it's you</p>
		<p>We're In This Together</p>
	</Slide>
</Slide>

<Slide backgroundImage="rollercoaster.jpg">
	<h2 class="bg-neutral-800/75">My Career</h2>
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
		<Notes>Testing notes</Notes>
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
	</Slide>
</Slide>
