# fitwow-web

Public marketing & legal site for FitWoW. Served via GitHub Pages at https://fitwow.net.

## Structure

```
/                         landing
/legal/about.html         shared About (company story)
/legal/ios/privacy.html   iOS Privacy Policy
/legal/ios/terms.html     iOS Terms of Service
/legal/android/...        Android (added when Android ships)
```

Why per-platform: legal text on each store mentions platform-specific systems (Apple App Store IAP / Sign in with Apple / HealthKit vs Google Play Billing / Health Connect). Mixing them confuses reviewers and can trip preflight rules.

## DNS

`fitwow.net` apex points to GitHub Pages IPs:

```
A @ 185.199.108.153
A @ 185.199.109.153
A @ 185.199.110.153
A @ 185.199.111.153
```

## Deploy

Push to `main` → GitHub Pages auto-builds. SSL via Let's Encrypt (auto).
