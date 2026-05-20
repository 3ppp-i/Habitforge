# HabitForge — Publishing Guide
## How to get your app on Google Play & Apple App Store

---

## STEP 1 — Host your app online (required for both stores)

You need your app accessible at a URL. Free options:

### Option A: Netlify (easiest — drag & drop)
1. Go to https://app.netlify.com
2. Sign up free
3. Drag the entire `habitforge-pwa` folder onto the Netlify dashboard
4. You'll get a URL like: https://habitforge-abc123.netlify.app
5. (Optional) Buy a custom domain like habitforge.app (~$10/year)

### Option B: GitHub Pages (free)
1. Create a free account at https://github.com
2. Create a new repository called "habitforge"
3. Upload all files from `habitforge-pwa/`
4. Go to Settings → Pages → Source: main branch
5. Your URL: https://yourusername.github.io/habitforge

---

## STEP 2 — Generate your APK & iOS package (free, no code)

1. Go to https://www.pwabuilder.com
2. Enter your hosted URL (from Step 1)
3. Click "Start" — PWABuilder will analyze your app
4. You'll see scores for Manifest, Service Worker, Security
5. Click "Build My PWA"
6. Choose "Android" → Download the APK package
7. Choose "iOS" → Download the iOS package
8. Both downloads are free

---

## STEP 3A — Publish to Google Play Store (Android)

### What you need:
- Google Play Developer account: https://play.google.com/console
- One-time registration fee: $25 USD
- The APK file from PWABuilder (Step 2)

### Steps:
1. Pay the $25 and create your developer account
2. Go to "Create app" in the Play Console
3. Fill in:
   - App name: HabitForge
   - Default language: English
   - App or game: App
   - Free or paid: Free
4. Upload your APK under "Production" → "Releases"
5. Fill in the store listing:
   - Short description (80 chars max): "Build daily habits, earn XP & level up your life with RPG progression"
   - Full description: (see below)
   - Screenshots: take 2-8 screenshots on your phone
   - Feature graphic: 1024x500 image
6. Set content rating (fill out questionnaire — it's for health/productivity)
7. Set pricing: Free
8. Submit for review → usually approved in 1-3 days

### Full description for Play Store:
HabitForge transforms your daily habits into an epic RPG adventure. Build powerful routines, earn XP for every habit completed, and rise through 10 dark fantasy warrior ranks from Iron Squire to Immortal God.

Features:
• Daily habit tracking with streaks & XP rewards
• 10 RPG warrior ranks with custom dark fantasy emblems
• Daily quests that refresh every midnight
• Full gym tracker — log sets, reps & weight
• 14 achievements to unlock
• Weekly progress charts & monthly activity heatmap
• Morning & evening reminders
• 3 visual themes: Dark Fantasy, Blood Red, Ocean Blue
• 100% offline — your data stays on your device

---

## STEP 3B — Publish to Apple App Store (iOS)

### What you need:
- Apple Developer account: https://developer.apple.com
- Annual fee: $99 USD/year
- The iOS package from PWABuilder (Step 2)
- A Mac computer with Xcode (OR use a cloud Mac service)

### No Mac? Use these cloud options:
- https://www.macincloud.com (~$1/hour)
- https://appcircle.io (has free tier)
- https://codemagic.io (free for open source)

### Steps:
1. Sign up at developer.apple.com and pay $99
2. Open the iOS package from PWABuilder in Xcode
3. Set your Bundle ID: com.yourname.habitforge
4. Set version: 1.0.0
5. Connect your Apple Developer account in Xcode
6. Archive the app (Product → Archive)
7. Upload to App Store Connect (https://appstoreconnect.apple.com)
8. Fill in the App Store listing:
   - Name: HabitForge
   - Subtitle: Level Up Your Daily Life
   - Category: Health & Fitness
   - Screenshots required: iPhone 6.7" and 6.5" sizes
9. Submit for review → usually 1-7 days

### App Store description:
HabitForge is the habit tracker that makes self-improvement feel like an adventure. Earn XP for every habit you complete, rise through dark fantasy warrior ranks, and conquer daily quests — all wrapped in a beautifully designed RPG experience.

---

## CHECKLIST before submitting

- [ ] App hosted at a public HTTPS URL
- [ ] Tested on real phone (Android & iOS)
- [ ] All icons look good on home screen
- [ ] Offline mode works (airplane mode test)
- [ ] Privacy Policy URL (required by both stores)
  → Free generator: https://www.privacypolicygenerator.info

---

## Privacy Policy (important!)

Both stores require a privacy policy. Since HabitForge stores all data locally on the device and doesn't collect any personal data, your policy can be very simple:

"HabitForge does not collect, transmit, or share any personal data. All user data is stored locally on the device. No accounts are required. No data leaves your device."

Generate a full one free at: https://www.privacypolicygenerator.info
Host it free at: https://www.netlify.com or GitHub Pages

---

## Quick summary

| Step | Android | iOS |
|------|---------|-----|
| Host app | Netlify (free) | Netlify (free) |
| Build package | PWABuilder (free) | PWABuilder (free) |
| Dev account | $25 one-time | $99/year |
| Review time | 1-3 days | 1-7 days |
| Needs Mac | No | Yes (or cloud Mac) |

Good luck, warrior! ⚔️
