# Privacy Policy — JacArrow

**Last updated:** 2026-05-15
**Data Controller:** Morten Jacobsen, Norway
**Contact:** galge.vender.0a@icloud.com

---

## Short version

JacArrow stores **all your data locally on your device**. We have no
servers that receive your shoots, sessions, or goals. When you uninstall
the app, all data is gone.

The only third parties that receive information are:
- **Apple** — handles App Store purchases and notifications
- **RevenueCat** (after you purchase Pro) — verifies your purchase

You have full GDPR rights to access, deletion, and data portability.

---

## What we store

### On your device (locally, never leaves the phone)
- **Shooting data:** sessions, rounds, arrow placements, scores, tags, goals, bows, and arrow sets
- **Settings:** selected language, theme, dominant hand, competition class, notification toggles
- **App history:** coach-mark status (which tips you have seen), tutorial-completed flags

All this data is stored in an SQLite database and AsyncStorage on your iPhone.
Neither JacArrow nor any third party has access to this data.

### iCloud (only when iCloud Drive is enabled)
JacArrow plans to use iCloud Key-Value Storage for one specific purpose:
to remember whether you have started the trial period before. This syncs
via your iCloud account to prevent uninstall + reinstall from granting a
new free trial period.

- Apple is the data processor (our agreement is governed by their standard terms)
- The values stored are **only**: the trial-start date and a «trial-used» status
- This feature activates when we launch the Pro model (Phase 4b)

If you have disabled iCloud Drive, or disabled iCloud Drive specifically
for JacArrow, iCloud is not used.

---

## Third parties

### Apple App Store
All in-app purchases are handled by Apple. We never receive card information,
addresses, or other payment details. Apple's
[Privacy Policy](https://www.apple.com/legal/privacy/) applies to the
purchase flow.

### Apple Push Notification Service (APNS)
JacArrow sends local notifications (PR achieved, trial-period expiration,
goal reminders). To deliver these, iOS registers an anonymous device token
with Apple. We have no servers sending push messages — all notifications are
generated locally on your device based on app state.

### RevenueCat (only after Pro purchase)
When you purchase JacArrow Pro, RevenueCat records your receipt and an
anonymous `appUserId` (a UUID generated on your device). This is necessary
for the app to verify your purchase on later use and during «Restore
Purchases». RevenueCat's
[Privacy Policy](https://www.revenuecat.com/privacy) applies. We never send
your name, email, or other personal data.

### Apple Analytics / Crash Reports
If you have enabled «Share App Analytics» in iOS Settings, Apple sends
anonymous aggregate data about usage and crashes to the developer.
JacArrow uses this for bug fixes and performance optimization. You can
disable this via:
**iOS Settings → Privacy & Security → Analytics & Improvements**.

---

## What we do NOT collect

- No user account, email address, or password
- No GPS or location data
- No access to contacts, calendar, camera, or microphone
- No third-party trackers (Firebase, Google Analytics, Facebook Pixel, etc.)
- No advertising identifiers (IDFA)
- No video tracking or device fingerprinting

---

## Your rights (GDPR)

You have the following rights under the General Data Protection Regulation:

**Right of access (Art. 15):** All your data is stored locally on your device.
You have full visibility via:
- Settings → My sessions (all historical rounds)
- Settings → My goals (all active and archived goals)
- Settings → Bows / Arrow sets / Locations (equipment management)

**Right to data portability (Art. 20):** Use
**Settings → Export my data** to download all your data as a JSON file. The
file can be shared via the iOS share sheet to email, AirDrop, Files, etc.
This is your complete shooting history in a standard format.

**Right to erasure (Art. 17):**
- *Delete individual session:* swipe the session on the home screen → Delete
- *Delete all data:* uninstall JacArrow — iOS automatically deletes all
  SQLite database and AsyncStorage. RevenueCat receipt (if you have
  purchased Pro) is retained by Apple and RevenueCat for refund and support
  purposes.

**Right to restriction and objection (Art. 18–21):** JacArrow does not
make any automated decisions about you. The Smart Insights engine only
analyzes your own training data locally on your device and presents
observations — it makes no decisions on your behalf.

**Right to withdraw consent (Art. 7):** Apple Analytics opt-in is controlled
via iOS Settings. RevenueCat data is deleted when you delete your Apple ID.

---

## Changes

We will update this policy when significant changes occur in how we process
data. Changes are communicated via:
1. «Last updated» date at the top of this page
2. In-app banner on first launch after update if the change is substantial
   (e.g. new third parties, new data collection)

---

## Complaints

If you believe we are processing your personal data in violation of GDPR,
you have the right to complain to your national data protection authority:

- **Norway:** [Datatilsynet](https://www.datatilsynet.no/)
- **EU/EEA:** find your authority at
  [edpb.europa.eu](https://www.edpb.europa.eu/about-edpb/about-edpb/members_en)

We encourage you to contact us first at galge.vender.0a@icloud.com — we take
all privacy inquiries seriously.
