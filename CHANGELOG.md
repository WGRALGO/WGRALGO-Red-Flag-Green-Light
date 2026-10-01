# Changelog

## v2.0.0 — 2026-10-01

- Version 2.0.0 (versionCode 200).
- The APK file is now named `WGRALGO-RedFlagGreenLight-v2.0.0.apk`. All WGRALGO apps now use the same `WGRALGO-<AppName>-v<version>.apk` naming.
- Works on phones and tablets in portrait and landscape. It rotates with your device, like the other WGRALGO apps.
- On phones turned sideways, the logo on the start screen is smaller, so the game starts on screen instead of below the logo.
- No changes to the questions, scoring, privacy, or license.

## v1.1.0 — 2026-10-01
- New question bank from the latest web version: 81 questions across
  Beginner, Everyday, and Expert, plus an All Levels round (easy to hard).
- Every round mixes 🚩 / 🟢 Red Flag or Green Light situations with 🧠 Know the
  basics questions; myth busters and "What to do" tips; results by topic.
- Real app look: black launch screen with the big logo (no white box on
  Android 12+), new launcher icon on black (the old icon background was
  white), solid app bar, and About / Privacy / Credits panels.
- Android back button asks before quitting a round, returns to the level
  picker from results, and asks before exiting.
- Removed the social, fundraising, and "Back to games" links from the new web
  version; a content security policy blocks all network access.
- The `INTERNET` permission that Capacitor merges in is now stripped from the
  final manifest.
- Signed with a new key. Uninstall v1.0.0 before installing v1.1.0.
- Added GitHub Actions debug builds and a signed release workflow with
  `tools/validate-release.sh`.

## v1.0.0
- Initial GitHub-ready Android APK release.
- Added offline investing education game.
- Added Multiple Choice and Opportunity / Trick question formats.
- Added score, streak, progress, instant feedback, and final rating.
- Added investing red flag explanations and learning tips.
- Removed website navigation, social media, and fundraising bars from APK interface.
- Added GPLv3 license, privacy statement, contributors file, and README.
