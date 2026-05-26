# WGRALGO Red Flag or Green Light: The Investing Reality Game

Red Flag or Green Light: The Investing Reality Game is a free educational Android app from The Wealth Gap Resolution Algorithm™ Inc. It helps users practice identifying real investing principles, risky money moves, hype, pressure tactics, and common investment red flags through interactive gameplay.

The app is fully offline, contains no ads, no analytics, no trackers, and asks for no permissions beyond what Android automatically grants.

---

## Features

- 30+ built-in investing-awareness scenarios
- Two question formats: **Multiple Choice** and **Opportunity or Trick** (red flag / green light)
- Real-time score, streak tracker, and progress bar
- Instant feedback with a short investing lesson after every question
- Final rating screen with replay option
- Premium black-and-gold WGRALGO design language
- Phone and tablet responsive layout
- Fully offline: no internet permission, no network calls
- No accounts, no ads, no analytics, no trackers

## Screenshots

Screenshots of the home, gameplay, feedback, and results screens are in [`/screenshots`](./screenshots).

## How to install / sideload the APK

1. Download `RedFlagGreenLight-v1.0.0.apk` from the [GitHub Releases](../../releases) page.
2. On your Android device, allow installs from your browser or file manager (Settings → Apps → Special access → Install unknown apps).
3. Open the downloaded APK and tap **Install**.
4. Optional integrity check (Linux/macOS):
   ```bash
   sha256sum RedFlagGreenLight-v1.0.0.apk
   ```
   Compare the output with `RedFlagGreenLight-v1.0.0.apk.sha256` from the same release.

## How to build from source

Requires Node.js 18+, Java 17, and the Android SDK.

```bash
git clone https://github.com/WGRALGO/WGRALGO-Red-Flag-Green-Light.git
cd WGRALGO-Red-Flag-Green-Light
npm install
npx cap sync android
cd android
./gradlew assembleDebug
```

The debug APK lands at `android/app/build/outputs/apk/debug/app-debug.apk`.

### Signed release build

Release signing uses `android/keystore.properties` **or** environment variables (`RFGL_KEYSTORE_FILE`, `RFGL_KEYSTORE_PASSWORD`, `RFGL_KEY_ALIAS`, `RFGL_KEY_PASSWORD`). The keystore and its passwords are **never** committed to git.

```bash
npx cap sync android
cd android
./gradlew assembleRelease
```

Output: `android/app/build/outputs/apk/release/app-release.apk`.

## Privacy summary

- No account required
- No ads
- No analytics
- No trackers
- No cloud upload
- No data selling
- No personal financial data is collected
- No answers or scores are sent to WGRALGO
- The app is an offline educational investing-awareness game

Full statement: [PRIVACY.md](./PRIVACY.md).

## Educational disclaimer

Red Flag or Green Light: The Investing Reality Game is for educational awareness only. It does not provide legal, financial, investment, tax, banking, brokerage, or professional advice. Investing involves risk, including possible loss of principal. No outcome in this app is a guarantee of future results. For personal financial decisions, consult a qualified professional.

## License

This project is released under the GNU General Public License v3.0. See [LICENSE](./LICENSE).

## Contributors

See [CONTRIBUTORS.md](./CONTRIBUTORS.md).
