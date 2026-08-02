# Privacy Policy for LinkSync

**Effective Date:** August 2, 2026

**Last Updated:** August 2, 2026

## In short

LinkSync converts music share links between Spotify and Apple Music. The core app runs entirely on your device and requires no account.

LinkSync also offers an **optional Premium subscription** that adds a private, synced history of the links people send you. Premium requires signing in with Apple and stores your history in your own account so it can sync across your devices. If you never sign in, LinkSync collects nothing about you — exactly as it always has.

This policy covers both.

## Who we are

LinkSync is developed and maintained by Alberto Paredes (referred to below as "we," "us," or "the developer"). For privacy matters we are the data controller. You can reach us at linksync.app@proton.me.

## The free app (no account)

Used without signing in, LinkSync behaves exactly as described in prior versions of this policy:

- It stores a few preferences **on your device** (your default service, your theme, and whether you've finished onboarding) using the operating system's standard storage (`UserDefaults` on iOS, `SharedPreferences` on Android). These never leave your device.
- To match a link across services it makes **unauthenticated** HTTPS requests to Spotify's and Apple's public lookup endpoints (details in "Third-party services" below). No identifier for you is sent.
- It does not create an account, and nothing about you is stored on any server.

You can use LinkSync this way forever. Everything in the next section applies **only if you choose to sign in for Premium.**

## LinkSync Premium (optional account)

When you sign in with Apple and use Premium, we create an account for you and store a history of your conversions so you can see who sends you music and keep that history across devices.

### What we collect and store

- **Account identifier.** Signing in with Apple gives us a stable, Apple-provided user identifier that we use as your account key. We request only your name from Apple. We do **not** ask Apple for your email; if you use Apple's Hide-My-Email relay, we never receive a real address.
- **Sender names you enter.** When you tag a converted link with the name of the person who sent it, we store that name (a label you type — we do **not** read your device's contacts or address book).
- **Conversion records.** For links you convert while signed in, we store the music link, the source and destination service, a search term derived from the link, the time, and whether the sender was confirmed by you or auto-attributed.
- **Subscription status.** To unlock Premium we record whether you hold an active subscription. The purchase itself is processed by Apple (or Google); we do not receive or store your payment card or billing details.

### Where it is stored and who processes it

Your Premium data is stored in a database and authentication service operated on our behalf by **Supabase, Inc.** as our data processor. Your subscription entitlement is managed through **RevenueCat, Inc.** Both act on our instructions under data-processing agreements.

- **In transit:** all traffic is encrypted over HTTPS.
- **At rest:** the database is encrypted, and access is protected by row-level security rules so that your rows are readable and writable **only** by your own authenticated account. No other user can access your data.

### What we still do not do

Even with Premium, LinkSync does **not**:

- Show ads or use any advertising identifier or ad network
- Use third-party analytics, telemetry, or cross-app tracking of any kind
- Access your contacts, calendar, photos, microphone, camera, or location
- Sell or rent your data to anyone

## Sign in with Apple

Premium uses Apple's "Sign in with Apple." Apple handles your credentials directly; we never see your Apple password. Apple's handling of your information is governed by [Apple's privacy policy](https://www.apple.com/legal/privacy/). We receive only the account identifier described above.

## Clipboard access

When you tap the paste button inside LinkSync, the app reads the current contents of your device clipboard so it can process the link you intend to convert. LinkSync does not read your clipboard passively or in the background. The clipboard contents are used only to extract a single music URL and are never stored or transmitted. On iOS 14 and later, your device shows a visual indicator whenever any app reads the clipboard; this is expected each time you tap paste.

## Third-party services

**Apple (iTunes Search API).** When you convert an Apple Music link, LinkSync sends a request to `https://itunes.apple.com/lookup?id=<track-id>&country=<storefront>`. The storefront is read from the Apple Music URL itself.

**Spotify (oembed endpoint).** When you convert a Spotify link, LinkSync sends a request to `https://open.spotify.com/oembed?url=<the link>`. This is Spotify's public, unauthenticated endpoint. Spotify's practices are governed by [Spotify's privacy policy](https://www.spotify.com/legal/privacy-policy/).

**Supabase (Premium only).** Authentication and storage for Premium accounts are provided by Supabase, Inc. See [Supabase's privacy policy](https://supabase.com/privacy).

**RevenueCat (Premium only).** Subscription entitlements are managed by RevenueCat, Inc. See [RevenueCat's privacy policy](https://www.revenuecat.com/privacy).

**What your IP address reveals.** As with any app that makes internet requests, the services above receive your device's public IP address, which is standard internet infrastructure. How they use it is described in their own privacy policies.

## Data retention and deletion

- **Free app:** preferences live only on your device and are removed when you delete the app or clear its data.
- **Premium:** your account data is kept until you delete it. You can permanently delete your account and **all** associated data at any time from within the app: **Settings → Account → Delete account**. This removes your account and every conversion record and sender name tied to it. You can also email us at linksync.app@proton.me to request deletion.

## International transfers

Our processors (Supabase and RevenueCat) are U.S.-based providers. If you access LinkSync from the European Union, United Kingdom, or European Economic Area, your Premium data may be processed outside your home country. Where required, such transfers are covered by Standard Contractual Clauses or equivalent safeguards under our agreements with those processors.

## Children

LinkSync is not directed to children under 13 (or the equivalent minimum age in your jurisdiction), and we do not knowingly collect information from children. If you believe a child has created a Premium account, contact us and we will delete it.

## Your rights

Because Premium means we now hold data about you when you're signed in, you have rights over it:

- **Access and portability** — ask us for a copy of your Premium data.
- **Correction** — sender names and tags are editable in the app; contact us for anything else.
- **Deletion** — delete your account in-app (**Settings → Account → Delete account**), or ask us to.

**European Union / United Kingdom / EEA (GDPR).** Our legal basis for processing Premium data is performance of the service you request (your subscription and history features). You may access, correct, delete, restrict, or object to processing, and lodge a complaint with your local supervisory authority. Contact us at linksync.app@proton.me.

**California (CCPA/CPRA).** We do not sell or share your personal information, and we do not use it for cross-context behavioral advertising. You may request access to or deletion of your information. Contact us at linksync.app@proton.me.

For the free app, these rights are satisfied by default because we hold no data about you.

## Changes to this policy

If LinkSync's behavior changes in a way that affects what information is accessed or how it is used, this policy will be updated and the "Last Updated" date above will change. Material changes will also be noted in the app's release notes on the App Store and Google Play.

## Contact

Questions about this policy or about LinkSync's privacy practices can be directed to linksync.app@proton.me.
