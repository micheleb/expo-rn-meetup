# expo-rn-meetup

Companion repo for the presentation I gave at the React Native Meetup on September 26, 2024 in Berlin.

Slides are based on the [Svelte reveal.js](https://github.com/micheleb/svelte-revealjs-slides-template) slides template I created based on [Create Beautiful Presentations With Svelte](https://www.youtube.com/watch?v=67lqa5kTQkA) by [Joy of Code](https://www.youtube.com/@JoyofCodeDev), with a few additions.

## See the slides

Clone the repo, then run

```bash
pnpm i
pnpm dev --open
```

(if you don't have `pnpm`, install it following [these instructions](https://pnpm.io/installation))

## Issues / Links I mentioned during the talk

- [EAS development builds don't work for both Simulators and Physical Devices at the same time](https://github.com/expo/expo/discussions/21121)
- [Provisioning profiles are invalidated every time they're pulled](https://github.com/expo/eas-cli/issues/1445)
- [Development builds cannot be distributed through TestFlight](https://expo.canny.io/feature-requests/p/dev-client-distribution-via-test-flight)
  - [Max](https://github.com/343max) presented his [`testflight-dev-deploy`](https://github.com/343max/testflight-dev-deploy) project in a lightning talk at the same meetup, what are the odds! ⚡
- The [Transporter app](https://apps.apple.com/us/app/transporter/id1450874784?mt=12) to submit your `.ipa` to the App Store
- The [Custom EAS updates server example](https://github.com/expo/custom-expo-updates-server)
- [My Personal Website](https://michelebonazza.com) :)
