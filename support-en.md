# Support — ArrowTrack

**Last updated:** 2026-05-20
**Version covered:** v1.0+
**Contact:** support@arrowtrack.app

---

## Quick help

### How do I record an end?

1. Open ArrowTrack → tap **New session** on the Home tab
2. Choose location, target face, and round format → tap **Start session**
3. **Tap on the target face** to place each arrow — use pinch-zoom and the precision loupe for accuracy
4. Tap **Save end** when all arrows are placed
5. Repeat for each end until the round is complete

### What's the difference between X and 10?

The X-ring is the innermost ring and scores 10 points — same as the 10-ring. ArrowTrack tracks X separately because X is used as the tiebreaker in competitions. Tap the «X» button when an arrow hits the X-ring in score-pad mode.

### How do I correct a misplaced arrow?

1. Long-press the arrow on the target → the precision loupe activates
2. Drag the arrow to the new position → release
3. OR tap the arrow to select → tap **Delete** to remove it

In score-pad mode: tap the arrow badge in the score-pad and select a new value.

### What's post-recording (the 📋 icon)?

The 📋 icon marks sessions that were entered manually using the score pad, not recorded on the target with coordinates. Hit map, constellation, and spread analysis are not available for post-recorded sessions — only the score totals.

### How do I buy Pro?

1. Tap any Pro-locked feature (e.g. a theme locked with a Pro badge)
2. Paywall appears with **Buy Pro (NOK 299)** button
3. Apple's standard purchase modal appears → confirm with Face ID / passcode
4. Pro activates immediately — all features unlock

**Price:** NOK 299 one-time purchase, lifetime. No subscription, no recurring charges.

### How do I restore purchases on a new iPhone?

1. Download ArrowTrack on the new iPhone (free version)
2. Sign in with the same Apple ID you used to buy Pro
3. Open ArrowTrack → **Settings → License → Restore Purchases**
4. Pro reactivates automatically

If you've changed Apple ID: contact support@arrowtrack.app and we'll help you.

### How do I export my data?

**Settings → About the app → Export my data** → iOS' share sheet appears. Choose AirDrop, Mail, Files, or wherever you want to send the JSON file.

The JSON contains all sessions, rounds, arrows, goals, bow setups, and settings — complete portability under GDPR Art. 20.

### How do I delete all my data?

Uninstall ArrowTrack → iOS automatically removes the entire SQLite database and all settings. No residual data remains on the device.

If you've bought Pro: the receipt remains with Apple (for refund and support purposes). Uninstall doesn't affect future re-installs — Pro reactivates automatically via Restore Purchases.

### Which round formats are supported?

- **WA 720** (outdoor, 6 ends × 12 arrows = 72 arrows)
- **WA 18 m Indoor** (10 ends × 3 arrows)
- **WA 1440** (4 sequential distances)
- **Vegas Shoot** (10 ends × 3 arrows indoor 18 m)
- **AGB Portsmouth** (10 ends × 3 arrows indoor 20 yd)
- **NFAA Indoor** (12 ends × 5 arrows indoor 20 yd)
- **Free Training** (no format limits)

All formats include official WA Book 3 compliance: line-breaking rule, separate X tracking, correct ring radii.

### Which target faces are supported?

- **WA 122 cm 10-ring** (outdoor standard)
- **WA 80 cm 10-ring** (outdoor long distance)
- **WA 40 cm 10-ring** (indoor single-spot)
- **WA 40 cm Vegas 3-spot triangular** (indoor competition)
- **WA 40 cm Vegas 3-spot vertical** (indoor alternative)
- **AGB Portsmouth 60 cm 10-ring** (indoor UK)
- **NFAA indoor single-spot blue 40 cm** (USA)
- **NFAA indoor 5-spot blue 40 cm** (USA competition)

---

## Technical issues

### The app crashes on launch

1. Turn iPhone off and on again
2. If still failing: uninstall and reinstall ArrowTrack (purchase data is NOT lost — receipt remains with Apple)
3. Send crash log to support@arrowtrack.app: **Settings → Privacy & Security → Analytics & Improvements → Analytics Data** → find the ArrowTrack log → share with us

If you've chosen to share analytics with the developer via iOS, crash logs are automatically sent to us.

### Score data disappeared after update

ArrowTrack stores everything locally in SQLite. Updates migrate the database forward-only — old data is converted to the new format, never deleted.

If you experience data loss:
1. Verify you're signed in with the same Apple ID
2. Check **Settings → About the app → Version number** — is it the latest?
3. Send us a description at support@arrowtrack.app

We have a strict rule that published migrations are immutable — data loss from updates should never happen. If it does, we have a bug and we want to hear about it.

### Pinch-zoom doesn't work on the target

1. Try with two fingers, not one
2. Check that you don't have «Reduce Motion» turned on in **iOS Settings → Accessibility → Motion** — it can limit gestures in some apps
3. Force-close the app (swipe up from the bottom, swipe ArrowTrack up) and reopen

### The constellation vibrates when dragging

This was a bug in v0.28.2 and earlier — fixed in v0.28.3. Update the app to the latest version in the App Store.

---

## Feedback and requests

### Suggest a new feature

Send an email to support@arrowtrack.app with:
- **What** you want (brief description)
- **Why** (what would it improve in your training?)
- **How often** would you use it (daily / per session / less frequently)

We read every single request and publish prioritized features in the app's «What's new» stream.

### Report a bug

Send an email to support@arrowtrack.app with:
- **What went wrong** (as detailed as you can)
- **What you expected to happen**
- **Step-by-step** to reproduce
- **iOS version** and **iPhone model** (Settings → General → About)
- **ArrowTrack version** (Settings → About the app)
- Screenshot if relevant

### General
We respond to all inquiries within 3 business days. Urgent issues (crashes preventing you from shooting) are prioritized higher.

---

## GDPR and privacy

For the full privacy policy: [Privacy](https://mjacobsen71.github.io/arrowtrack-legal/privacy-en)

To export your data, delete a session, or exercise other GDPR rights: see the Privacy Policy.

Privacy complaints: contact us at support@arrowtrack.app **first**. If we can't resolve the matter, you can complain to your national data protection authority. For Norway: [Datatilsynet](https://www.datatilsynet.no/).

---

## About ArrowTrack

**Developer:** Morten Jacobsen, Norway
**Homepage:** [mjacobsen71.github.io/arrowtrack-legal](https://mjacobsen71.github.io/arrowtrack-legal)
**Privacy Policy:** [Privacy](https://mjacobsen71.github.io/arrowtrack-legal/privacy-en)
**Licenses (open source):** See Settings → About the app → Licenses in the app

ArrowTrack is a solo-developer project built for archers at every level — from your first arrow to your hundredth tournament. WA Book 3 compliant scoring is there from day one, ready when you want it. Built with React Native + Expo + TypeScript + SQLite. No backend, no cloud, no tracking.

Thanks for using the app. 🏹
