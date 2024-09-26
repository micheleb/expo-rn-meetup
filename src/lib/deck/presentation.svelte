<script lang="ts">
	import Code from './code.svelte';
	import Fragment from './fragment.svelte';
	import Markdown from './markdown.svelte';
	import Notes from './notes.svelte';
	import Slide from './slide.svelte';
	import TT from './tt.svelte';
</script>

<Slide backgroundImage="title-bg.jpg">
	<h1>Things that ChatGPT won't tell you about Expo</h1>
</Slide>

<Slide>
	<Slide animate>
		<h2>Talking About</h2>
	</Slide>

	<Slide animate uncounted>
		<Notes>
			<ul>
				<li>How many have used Expo?</li>
				<li>How many in prod now?</li>
			</ul>
		</Notes>
		<h2>Talking About</h2>
		<p>Expo (duh)</p>
	</Slide>

	<Slide animate uncounted>
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

	<Slide animate uncounted>
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

	<Slide animate uncounted>
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
	<Notes>
		<ul>
			<li>Started as a Backend dev</li>
			<li>Moved on to FullStack</li>
			<li>Then React Native</li>
		</ul>
	</Notes>
</Slide>

<Slide>
	<Slide animate>
		<Notes>
			<ul>
				<li>URBI in 2018</li>
				<li>Ditto in 2019</li>
				<li>JW TVs in 2021, no luck until very recently</li>
				<li>JW Mobile in 2022</li>
			</ul>
		</Notes>
		<h2>RN, Expo, and I</h2>
		<Fragment>Started 6 years ago 👴</Fragment>
		<Fragment>2018: Expo 27 <Fragment inline>❌</Fragment><Fragment animation="fade-in-then-semi-out" inline>{' '}(<TT>react-native-maps</TT>)</Fragment></Fragment>
		<Fragment>2019: Expo 33 <Fragment inline>❌</Fragment><Fragment animation="fade-in-then-semi-out" inline>{' '}(<TT>crypto-js</TT>)</Fragment></Fragment>
		<Fragment>2021: 📺 <Fragment inline>❌</Fragment><Fragment animation="fade-in-then-semi-out" inline>{' '}(no TVs until recently)</Fragment></Fragment>
		<Fragment>2022: Expo 44 ... 48 <Fragment inline>✅</Fragment><Fragment animation="fade-in-then-semi-out" inline>{' '}(DS showcase)</Fragment></Fragment>
		<Fragment>Now on Expo 51 🚀</Fragment>
	</Slide>
</Slide>

<Slide>
	<Slide animate>
		<h2>Expo Go</h2>
		<img src="expo-go.png" alt="The Expo Go app" class="object-none pl-24" />
	</Slide>

	<Slide animate>
		<h2>Expo Go</h2>
	</Slide>

	<Slide animate>
		<h2>Expo Go</h2>
		<p>Very nice for prototypes</p>
	</Slide>

	<Slide animate>
		<h2>Expo Go</h2>
		<p>Very nice for prototypes</p>
		<p>Expo is gently shooing us off</p>
	</Slide>
	<Slide animate>
		<h2>Expo Go</h2>
		<p>Very nice for prototypes</p>
		<p>Expo is gently shooing us off 😅</p>
		<p>Go go <span class="text-heading-color">development builds</span></p>
	</Slide>
</Slide>

<Slide>
	<Slide animate>
		<h2>Development builds</h2>
	</Slide>

	<Slide animate>
		<h2>Development builds</h2>
		<p>Your app + Expo Go</p>
	</Slide>

	<Slide animate>
		<h2>Development builds</h2>
		<p>Your app + Expo Go</p>
		<p>Needed for libraries with native code</p>
	</Slide>

	<Slide animate>
		<h2>Development builds</h2>
		<p>Your app + Expo Go</p>
		<p>Needed for libraries with native code</p>
		<p>Use native code using <span class="text-heading-color">Expo modules</span></p>
	</Slide>

	<Slide animate>
		<h2>Development builds</h2>
		<p>Your app + Expo Go</p>
		<p>Needed for libraries with native code</p>
		<p>Use native code using <span class="text-heading-color">Expo modules</span></p>
		<p>Write your own native code with <span class="text-heading-color">Expo local modules</span></p>
	</Slide>
</Slide>

<Slide>
	<Slide animate>
		<h2>Eas build</h2>
	</Slide>

	<Slide animate>
		<h2>Eas build</h2>
		<p>Build your app on Expo servers 💸</p>
		<Notes>
			Expo has a free tier, but you get queued, especially on iOS
		</Notes>
	</Slide>

	<Slide animate>
		<h2>Eas build</h2>
		<p>Build your app on Expo servers 💸</p>
		<p>...or locally with <TT>--local</TT>💡</p>
	</Slide>

	<Slide animate>
		<h2>Eas build</h2>
		<p>Build your app on Expo servers 💸</p>
		<p>...or locally with <TT>--local</TT>💡</p>
		<p>(or on your own CI)</p>
	</Slide>

	<Slide animate>
		<h2>Eas build</h2>
		<p>Build your app on Expo servers 💸</p>
		<p>...or locally with <TT>--local</TT>💡</p>
		<p>(or on your own CI)</p>
		<p>use <TT>eas.json</TT> to set it up</p>
	</Slide>
</Slide>

<Slide backgroundImage="hangover-math.gif">
	<h1 class="bg-neutral-800/35">eas.json</h1>
		<Notes>docs are unopinionated, here's my take</Notes>
</Slide>

<Slide>
	<Slide animate>
		<h3>eas.json</h3>
		<Code id="code" lines="|3,4|7-11|7,8">
			{`
{
  "cli": {
    "version": ">= 4.1.2",
    "appVersionSource": "remote"
  },
  "build": {
    "development": {/* ... */},
    "simulator": {/* ... */},
    "preview": {/* ... */},
    "beta": {/* ... */},
    "production": {/* ... */}
  },
  "submit": {
    "beta": {},
    "production": {}
  }
}
    `}
		</Code>
		<Notes>
			<ul>
				<li>version, will discuss later</li>
				<li>dev and simulator: your local builds</li>
			</ul>
		</Notes>
	</Slide>

	<Slide animate>
		<Notes>
			<ul>
				<li>on iOS, you can either build for a physical device OR the simulator</li>
			</ul>
		</Notes>
		<h3>eas.json</h3>
		<Code id="code" lines>
			{`
{
  "cli": {/* ... */},
  "build": {
    "development": {
      "developmentClient": true,
      "distribution": "internal",
      "channel": "development",
      "autoIncrement": true
    },
    "simulator": {
      "extends": "development",
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
		<Notes>
			<ul>
				<li>Distribute APKs to anybody</li>
				<li>For iOS you need people in your team with their Apple accounts, or an Open Beta (reviewed) and invites (up to 1k)</li>
				<li>linked issue with provisioning, use spacebar to select multiple devices</li>
				<li>channel for eas update</li>
				<li>env to creates different apps (packageId, bundleId)</li>
			</ul>
		</Notes>
		<h3>eas.json</h3>
		<Code id="code" lines="16-26|21|18-20">
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
      "extends": "development",
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

<Slide>
	<Slide animate>
		<h3>app.config.js</h3>
		<Notes>
			<ul>
				<li>Secrets are not available on local builds</li>
				<li>eas uses .gitignore for files, so you need to add it to ~/.gitignore (~/.gitconfig core excludesFile)</li>
			</ul>
		</Notes>
		<Code id="code" lines="1|4,7,12|16-21|9-11">
			{`
const IS_PROD = process.env.APP_VARIANT === "production";

export default {
  android: {
    adaptiveIcon: {
      backgroundColor: "#e6a482",
      foregroundImage: \`./assets/icon\${IS_PROD ? "" : "-dev"}.png\`,
    },
    googleServicesFile: IS_PROD
      ? process.env.GOOGLE_SERVICES_JSON || "./google-services.json"
      : process.env.GOOGLE_SERVICES_JSON_DEV || "./google-services-dev.json",
    package: \`com.my.app\${IS_PROD ? "" : ".dev"}\`,
		/* ... */
  },
	/* ... */
  icon: \`./assets/icon\${IS_PROD ? "" : "-dev"}.png\`,
  ios: {
    bundleIdentifier: \`com.my.app\${IS_PROD ? "" : ".dev"}\`,
		/* ... */
  },
  name: \`My App\${IS_PROD ? "" : " Test"}\`,
	/* ... */
`}
		</Code>
	</Slide>
</Slide>
