# Privacy Policy for LinkSync

**Effective Date:** May 22, 2026

**Last Updated:** May 22, 2026

## In short

LinkSync converts music share links between Spotify and Apple Music. It runs entirely on your device. We do not operate a server, we do not create accounts, and we do not collect, store, or transmit any information about you.

## Who we are

LinkSync is developed and maintained by Alberto Paredes (referred to below as "we," "us," or "the developer"). You can reach us at linksync.app@proton.me.

## What information we collect

**None that leaves your device.**

LinkSync stores a small number of preferences on your device using the operating system's standard preferences storage. On iOS these are stored via `UserDefaults`; on Android these are stored via `SharedPreferences`. The preferences we store are:

- Your chosen default service (Spotify or Apple Music)
- Your theme preference
- Whether you have completed the first-run onboarding

These values never leave your device. They are removed when you uninstall LinkSync or clear the app's data through your device settings.

## What information we do not collect

We want to be explicit about what is not happening. LinkSync does not:

- Require or create user accounts
- Collect your name, email address, phone number, or any other personal identifier
- Collect your location
- Access your contacts, calendar, photos, microphone, or camera
- Use analytics services (no Google Analytics, no Firebase Analytics, no Mixpanel, no Amplitude, no third-party telemetry of any kind)
- Use crash reporting services that transmit crash logs to third parties
- Use advertising identifiers or integrate with advertising networks
- Use cross-app tracking or device fingerprinting
- Sell your data to anyone (we have no data to sell)

## Clipboard access

When you tap the paste button inside LinkSync, the app reads the current contents of your device clipboard so it can process the link you intend to convert. LinkSync does not read your clipboard passively or in the background. The clipboard contents are used only to extract a single music URL and are never stored or transmitted.

On iOS 14 and later, your device will display a visual indicator whenever any app reads the clipboard. This is normal and expected behavior each time you tap our paste button.

## Third-party services

LinkSync makes unauthenticated HTTPS requests to two public third-party endpoints in order to look up track, album, or playlist metadata so the app can build a matching search on the other service. No identifier for you is sent in either request.

**Apple (iTunes Search API).** When you paste an Apple Music link, LinkSync sends a request to `https://itunes.apple.com/lookup?id=<track-id>&country=<storefront>`. The storefront value is read from the Apple Music URL itself (for example `us`, `gb`, or `jp`). Apple's own privacy practices are governed by Apple's privacy policy at [apple.com/legal/privacy](https://www.apple.com/legal/privacy/).

**Spotify (oembed endpoint).** When you paste a Spotify link, LinkSync sends a request to `https://open.spotify.com/oembed?url=<the link you pasted>`. This is Spotify's public, unauthenticated oembed endpoint. Spotify's own privacy practices are governed by Spotify's privacy policy at [spotify.com/legal/privacy-policy](https://www.spotify.com/legal/privacy-policy/).

**Opening converted links.** When you tap "Open in Spotify" or "Open in Apple Music," LinkSync hands the destination URL to your device's default browser or to the installed Spotify or Apple Music app using the operating system's standard URL handler. From that point forward, the privacy policy of the receiving service — Spotify, Apple, or your browser vendor — applies instead of ours.

**What your IP address reveals.** As with any app that makes internet requests, the third-party services above receive the request from your device's public IP address, which is standard internet infrastructure. We do not see this information and we do not store it. How those services use the IP addresses they receive is described in their own privacy policies, linked above.

## Children

LinkSync is not directed to children under 13 (or the equivalent minimum age in your jurisdiction) and we do not knowingly collect any information from children. Because LinkSync does not collect information from anyone, no information from children is collected either.

## Your rights

Because LinkSync stores nothing on any server, there is nothing for us to access, export, correct, or delete on your behalf. You can exercise full control over all LinkSync data by:

- Deleting the app, which removes all stored preferences from your device, or
- Clearing the app's data through your device settings, which has the same effect.

**If you are in the European Union, United Kingdom, or European Economic Area.** The General Data Protection Regulation (GDPR) grants you rights regarding personal data held by organizations. Because LinkSync does not hold any personal data about you on any server, these rights are satisfied by default. If you have questions about your rights under GDPR in relation to LinkSync, you can contact us at linksync.app@proton.me.

**If you are a California resident.** The California Consumer Privacy Act (CCPA) and California Privacy Rights Act (CPRA) grant you rights regarding personal information. LinkSync does not collect, sell, or share personal information. If you have questions about your rights under CCPA or CPRA in relation to LinkSync, you can contact us at linksync.app@proton.me.

## Changes to this policy

If LinkSync's behavior changes in a way that affects what information is accessed or how it is used, this policy will be updated and the "Last Updated" date above will change. Material changes will also be noted in the app's release notes on the App Store and Google Play.

## Contact

Questions about this policy or about LinkSync's privacy practices can be directed to linksync.app@proton.me.
