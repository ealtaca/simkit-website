# Privacy Policy for SimKit

**Last Updated: October 30, 2026**

## Introduction

SimKit ("we," "our," or "us") is a free macOS app for working with the iOS Simulator. This Privacy Policy explains what SimKit sends off your Mac, what stays on it, and how to turn data collection off.

**In short:** the network traffic, tokens, mocks and captures you work with in SimKit never leave your Mac. SimKit sends anonymous usage data to Google Firebase, including the bundle IDs of the apps you debug, and you can turn that off.

## What Stays on Your Mac

Everything you work with in SimKit is stored and processed locally:

- Network requests and responses captured from the Simulator, including headers, bodies and tokens
- Mock endpoints, throttling profiles, GPX routes and other configurations
- Screenshots, videos and GIFs you capture
- App preferences

This data is never sent to us or to any third party. It is deleted when you delete it in the App or remove SimKit and its data from your Mac.

The SimKit SDK, if you add it to your app, talks only to SimKit on the same Mac over the local loopback address (127.0.0.1). It contains no analytics and sends nothing to us.

## What SimKit Sends

### Anonymous Usage Data (Google Firebase)

Unless you turn it off, SimKit sends the following to Google Firebase Analytics:

- **Feature usage**: which tools and tabs you open, captures and exports you make, onboarding steps
- **Errors**: error messages from SimKit and the last few actions that led to them
- **Simulator details**: the bundle IDs of the apps you select in the Simulator (for example `com.example.myapp`) and the names of simulated devices (for example "iPhone 17 Pro")
- **Your Mac**: macOS version, chip, memory, screen size, SimKit version
- **Standard Firebase data**: a random app instance ID, session counts and length, and an approximate country derived from your IP address

SimKit also writes a small usage report to Google Cloud Firestore: the bundle ID of an app you debugged, a random ID generated for your installation, the day, and the SimKit version. At most one report is written per app per day. The App can only create these reports; it cannot read them back.

**We do NOT collect:** your name, email address or Apple ID, the contents of any network traffic, tokens, files, screenshots or recordings.

### Update Checks

- SimKit reads the latest SDK version from Google Cloud Firestore so it can tell you when a new SDK is available. Nothing about you is written in this check.
- The DMG version checks for app updates with Sparkle by downloading our appcast from GitHub (ealtaca.github.io). As with any download, GitHub sees your IP address. The Mac App Store version is updated by Apple.

## How to Turn It Off

In SimKit, open **Settings > General** and turn off **Share anonymous usage data**. This stops both the Firebase events (including Firebase's own automatic ones) and the Firestore usage reports. If your version of SimKit does not have this setting yet, update to the latest version, or email us and we will delete the data we hold.

## How We Use the Data

1. **Improve the app**: learn which features are used and which are not
2. **Fix bugs**: find errors and the steps that cause them
3. **Decide what to build**: see what kinds of apps SimKit is used on

We do not use it for advertising, and we do not sell, rent or share it with anyone for marketing.

## Third-Party Services

- **Google Firebase** (Analytics, Cloud Firestore): [Firebase Privacy and Security](https://firebase.google.com/support/privacy)
- **GitHub** (hosts DMG downloads and the update feed): [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)
- **Apple** (Mac App Store distribution): [Apple Privacy Policy](https://www.apple.com/privacy/)

SimKit 1.6 and earlier, from the Mac App Store, also included RevenueCat for a Pro subscription. SimKit is now free; RevenueCat was removed in version 1.7.

## Data Retention

- **Firebase Analytics**: kept for up to 14 months, then deleted by Google
- **Firestore usage reports**: kept while they are useful for product decisions; we will delete them on request
- **Local data**: kept on your Mac until you delete it

## Permissions Required

SimKit requests the following macOS permissions:

- **Screen Recording**: To detect active simulator windows and position the floating panel alongside them. Only window metadata (position, size, title) is read — no screen content is captured, stored, or transmitted. Window metadata is held in memory while the App runs and is never written to disk.
- **Accessibility**: To detect and interact with simulator windows
- **File Access**: To save screenshots and videos to your chosen location (~/Downloads by default)
- **Network (Local)**: To communicate with the SimKit SDK running inside the Simulator over the local loopback address

These permissions are only used for the App's core functionality and can be revoked in System Settings at any time.

## Your Rights

Wherever you live, you can ask us to access or delete the data we hold about you, or object to its processing, by emailing **ealtaca@gmail.com**. Because the data is anonymous, we may ask you for your SimKit version and roughly when you used it so we can find it.

**EU and UK users (GDPR):** we process usage data on the basis of our legitimate interest in improving SimKit. You have the right to access, rectify, erase, restrict and port your data, and to object to processing. You may also complain to your data protection authority.

**California users (CCPA):** you have the right to know what personal information is collected and to request its deletion. We do not sell or share personal information.

## Children's Privacy

SimKit is a developer tool and is not intended for children under 13. We do not knowingly collect information from children.

## International Users

SimKit is developed in Turkey. Google Firebase and GitHub may process data in other countries, including the United States.

## Changes to This Policy

We will update the date at the top of this page when this policy changes, and note material changes in the App's release notes.

## Contact Us

**Email:** ealtaca@gmail.com
**GitHub Issues:** [github.com/ealtaca/simkit-website/issues](https://github.com/ealtaca/simkit-website/issues)
**Developer:** Emre Can Altaca

We will respond to all requests within 30 days.

---

**Effective Date:** October 30, 2026
