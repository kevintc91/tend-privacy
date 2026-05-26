# Privacy Policy for Tend

**Effective date:** May 26, 2026
**Last updated:** May 26, 2026

This is the privacy policy for **Tend**, a daily Stoic philosophy app published by Kevin Childers (the "developer," "we," or "us"). This policy explains what information Tend collects, what it doesn't, and what your rights are.

We've kept it short on purpose. Tend is built to be privacy-friendly: most of what you do in the app never leaves your phone, and the small amount of data the app does send is anonymous and minimal.

If you have questions about anything here, email **tendadmin@gmail.com**.

---

## The short version

- Your journal entries never leave your phone.
- The app does not require an account, email, name, or any login.
- The app collects no advertising identifiers, no location, no contacts, no analytics, and no device fingerprints.
- The only thing the app sends to a server is **anonymous feedback** on individual quotes (a vote of "landed" or "didn't land," an optional reason, and basic app metadata), and only when you have the feedback toggle on in Settings.
- You can turn that toggle off at any time. With it off, the app sends nothing.

If that's enough for you, you're done. The rest of this document is the detail.

---

## 1. Who this policy covers

This policy applies to the Tend mobile application, distributed via the Apple App Store and the Google Play Store. If a future version of Tend introduces accounts, cloud sync, or community features, this policy will be updated and a clear notice will appear in the app before any new data collection begins.

This policy does not cover any third-party app stores, operating systems, or device platforms (Apple, Google) that distribute or run Tend. Those parties have their own privacy policies, and we recommend reading them.

---

## 2. Data we do not collect

To be explicit, Tend does not collect any of the following:

- Your name, email address, phone number, or any other contact information
- Your date of birth, gender, or any other demographic information
- Your location (the app never requests location permission)
- Your contacts, calendar, photos, microphone, or camera
- Your IP address (Tend's backend does not log IP addresses; see Section 5)
- Any advertising identifier (IDFA on iOS, AAID on Android)
- Any device fingerprint, install ID, or persistent unique identifier we control
- Any analytics or behavioral telemetry (Tend does not use Google Analytics, Mixpanel, Sentry, Firebase Analytics, or any similar SDK)
- The text of any reflection you write in the journal
- Any record of which quotes you have viewed, journaled on, or skipped

---

## 3. Data stored locally on your phone

The following data is stored **only on your device**, using your phone's local storage. It is not transmitted to the developer or to any third party.

- **Journal entries.** Every reflection you save in Tend is written to your phone's local storage, indexed by the quote it belongs to and the date you saved it. We never see this text. It is never uploaded.
- **Notification settings.** Your chosen delivery time and on/off toggle for the daily reminder are stored locally so the app can schedule the local notification at the right time. No notification scheduling involves a server.
- **Onboarding flag.** A single boolean indicating whether you have completed the first-run onboarding flow.
- **Feedback toggle state.** Whether you have anonymous feedback turned on or off in Settings.
- **Local vote cache.** A record of which quotes you have already given feedback on, so the in-app prompt doesn't reappear. This cache contains the same information that is uploaded as anonymous feedback (Section 4); it stays on your device as well so the UI works offline.

If you uninstall Tend, all of this local data is deleted along with the app, per the platform's standard uninstall behavior. Backups to iCloud or Google Drive may preserve this data; that backup is governed by Apple's or Google's privacy practices, not ours.

---

## 4. Anonymous feedback (the only data Tend sends to a server)

Tend has an in-app prompt below each daily quote asking whether the quote "landed" or "didn't land," with an optional follow-up asking what specifically didn't land. This data helps us identify quotes whose translations or examples aren't working and rewrite them in future updates.

When you submit feedback **and** you have the feedback toggle on in Settings (the default), the app sends the following to our backend:

- The internal ID of the quote (a number like `042`, with no information about you attached)
- Your vote: either `landed` or `didnt_land`
- The optional reason you selected, if any (one of: translation off, translation unclear, example irrelevant, reflection forced, didn't resonate)
- The version of the Tend app installed (for example, `1.0.0`)
- The platform you are on (`ios` or `android`)

That is the entire payload. There is no user ID, no device ID, no IP address logged, no timestamp tied to anything that could identify you, no journal text, no reading history, and no list of which quotes you have or have not seen.

You can turn feedback off in **Settings → Feedback → Help improve Tend's content**. With it off, the app sends nothing, regardless of what you do in the in-app prompt. (The local vote cache still records that you voted, so the prompt doesn't keep appearing.)

---

## 5. Where anonymous feedback is stored

The anonymous feedback described in Section 4 is stored in a database hosted by **Supabase, Inc.** (the "processor"). Supabase is a US-based managed-database provider. Their privacy policy is at [https://supabase.com/privacy](https://supabase.com/privacy).

The Tend developer has access to the contents of this database in order to read aggregate feedback and improve the app's content. The developer does **not** receive any other information about you from Supabase.

Supabase, as the database operator, may log standard request metadata such as the IP address from which the database is accessed. Because the app sends feedback directly from your device, this means Supabase may technically log the IP address that submitted the feedback. The developer does not query, store, or use this metadata. We are working on routing feedback through a proxy that strips IP addresses before they reach Supabase; until that ships, this is the most accurate description.

If you want to avoid any data leaving your device, set the feedback toggle to off.

---

## 6. Data we do not share

The developer does not sell, rent, trade, or otherwise share any data (including the anonymous feedback) with any party other than the Supabase processor described in Section 5. There is no advertising network, marketing partner, data broker, or analytics company involved in Tend.

If law enforcement issues a valid legal request for data that Tend possesses, the developer will respond as required by applicable law. Note that the data Tend possesses is anonymous and minimal (Section 4), so such a request would not yield personally identifying information.

---

## 7. Data retention

The anonymous feedback described in Section 4 is retained indefinitely, in aggregate, in order to inform future improvements to Tend's content. Because the data contains no personally identifying information, there is no person to delete a record about. If you want to "delete" your feedback, the practical action is to turn the feedback toggle off in Settings; the existing anonymous records cannot be linked back to you.

Local data on your phone (Section 3) is retained until you uninstall the app, clear app data, or delete it through the app's interface (in a future version, individual journal entries will be deletable from within Tend).

---

## 8. Children's privacy

Tend is intended for users **age 13 and older**. The app does not knowingly target or collect data from children under 13. Because Tend collects no personally identifying information from anyone, the practical risk to any user under 13 is low, but the app is not marketed to children and the content is written for adult readers.

If you are a parent or guardian and you believe a child under 13 has used Tend, contact tendadmin@gmail.com and the developer will assist where possible.

---

## 9. Your rights

### If you are in the European Economic Area, the United Kingdom, or Switzerland (GDPR)

Under the General Data Protection Regulation (GDPR), you have the right to:

- Be informed about what data is collected (this policy)
- Access any personal data we hold about you
- Request correction or deletion of any personal data we hold about you
- Object to or restrict processing of your personal data
- Receive your personal data in a portable format
- Lodge a complaint with your local data protection authority

Because Tend collects no personally identifying information, in practice there is no "personal data" the developer holds about you that could be accessed, corrected, deleted, or ported. If you believe otherwise, or you want to discuss it, email tendadmin@gmail.com.

The legal basis for processing the anonymous feedback (Section 4) is your consent (you can disable it at any time in Settings) and the developer's legitimate interest in improving the app's content.

### If you are a California resident (CCPA / CPRA)

Under the California Consumer Privacy Act (CCPA) and the California Privacy Rights Act (CPRA), you have the right to:

- Know what personal information is collected about you
- Know whether your personal information is sold or disclosed (it is not)
- Say no to the sale of your personal information (the developer does not sell any data)
- Access your personal information
- Request deletion of your personal information
- Not be discriminated against for exercising these rights

As with GDPR, Tend collects no personally identifying information, so in practice there is no personal information for the developer to access, sell, or delete. If you have questions, email tendadmin@gmail.com.

---

## 10. International data transfers

If you use Tend outside the United States, your anonymous feedback (Section 4) is transmitted to and stored on servers operated by Supabase in the United States. The legal basis for this transfer, where applicable, is your consent and the developer's legitimate interest in improving the app's content.

---

## 11. Security

The developer uses standard industry practices to protect the small amount of anonymous data Tend sends to its backend. The connection between your phone and the backend is encrypted in transit (HTTPS / TLS). The backend database is hosted by Supabase, which uses encryption at rest and standard cloud security controls.

No system is 100 percent secure. The best protection for your data is the design choice that most of it never leaves your phone in the first place.

---

## 12. Third-party services

Tend uses the following third-party services. None of them receive personally identifying information.

- **Apple Push Notification service and Google's notification system.** Tend uses local notifications scheduled on your device. These are delivered by the operating system's own notification subsystem. The developer does not operate a push-notification server, and no notification content is generated remotely.
- **Apple App Store / Google Play Store.** When you install Tend, the relevant store provides the developer with aggregated, anonymized installation and crash statistics. The developer does not receive a list of installers or any identifying information about installers.
- **Supabase.** See Section 5.

---

## 13. Changes to this policy

If this privacy policy materially changes, the new version will be published at this URL and the "Last updated" date at the top will reflect the change. For changes that introduce new data collection (for example, if a future version of Tend adds user accounts or cloud sync), the app will display an in-app notice and require fresh consent before any new data is collected.

For minor edits (typo fixes, clarifications, contact info updates), the date at the top will be updated without further notice.

---

## 14. Contact

Questions about this policy, requests under GDPR or CCPA, or concerns about data handling:

**Email:** tendadmin@gmail.com
**Developer:** Kevin Childers
**App:** Tend
