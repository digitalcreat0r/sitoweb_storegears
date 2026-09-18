---
layout: document
title: Privacy Policy - ScreenRest
back_url: /
back_text: Back to Home
---
# Privacy Policy - ScreenRest

*Last updated: September 5, 2026*

**ScreenRest** is an application developed and managed by **{{ site.author }}** ("the developer"), operating as **{{ site.brand }}**. It is built with a "Privacy by Design" approach. This application is designed to function primarily on your device while maintaining high standards for technical stability and privacy.

## 1. Data Controller
The data controller for this application is:

**{{ site.author }} ({{ site.brand }})**

Email: {{ site.email }}<br>
Website: {{ site.url }}

## 2. Information Collection
The developer does **not** collect, store, or process any personal information such as names, email addresses, or phone numbers by default.

### Support & Feedback (Voluntary)
If you choose to contact the developer via the "Support" or "Feedback" features, you may voluntarily provide your name and email address. This information, along with essential technical details (such as app version, device model, and Android version), is used solely to respond to your request and resolve technical issues. These details are not used for any other purpose.

### App Improvement & Analytics (Opt-In)
To understand how the app is used and improve its features, **Firebase Analytics** is used. By default, this collection is **disabled**.
- **Consent:** After the initial setup, you will be asked for explicit consent to share anonymous usage data. You can also change this preference at any time in the app **Settings**.
- **Data Collected:** The developer collects only anonymous events (such as opening the app, viewing specific screens like "Home" or "Settings", and completing the setup) to help the developer identify which features are most valued by users. No personal or identifying data is ever associated with these events.

### Diagnostics & Crash Reporting (Opt-In)
To help improve app stability, **Firebase Crashlytics** is used. By default, automatic crash reporting is disabled.

In the event of a crash, a local log is generated on your device. Upon your next launch, you will be presented with a prompt asking for your explicit consent to send this specific crash report.
- **If you choose "Send":** The app will transmit the anonymous report to Firebase.
- **If you choose "Don't Send":** The local report is permanently deleted from your device and no data is transmitted.

The anonymous report, only if explicitly sent by you, includes:
- **Crashlytics Installation UUID:** A randomly generated, anonymous identifier.
- **Stack traces:** Technical logs indicating exactly where the code failed.
- **Device Metadata:** Hardware model, operating system version, and the state of the app at the time of the crash.

### Third-Party Services
- **Google Play Services:** Used for age verification signals and basic app functionality. Google may process data according to their own [Privacy Policy](https://policies.google.com/privacy).

## 3. Age Verification & Minor Protection
To comply with regional regulations (such as the Texas SCOPE Act), ScreenRest implements age verification measures:
- **Automated Verification:** The app uses Google Play Age Signals to determine if a user is a minor or an adult based on their Google account status. This process is handled by Google Play Services; the developer only receives an anonymous status signal (e.g., "Verified Adult" or "Supervised Minor") and does not access your date of birth or identity documents.
- **Manual Declaration:** If automated verification is unavailable, users must manually declare their age category.
- **Minor Safety:** For users identified as minors, the app requires a manual acknowledgment of parental guidance. Since ScreenRest collects no personal data and operates entirely offline, it does not create "digital service provider" profiles for minors.

## 4. Local Storage & Permissions
The app uses **Android Jetpack DataStore** to save your preferences locally. These remain on your device and are never uploaded to any external server.
- **Age Verification Status:** Your age category (Adult/Minor) is stored locally using Android Jetpack DataStore to remember your status and avoid repeated prompts. This data never leaves your device.

### Permissions Used
- **Exact Alarms:** Used to trigger precise wellness timers.
- **Notifications:** Used to provide status updates and reminders.
- **Vibration:** Used for haptic feedback.

## 5. Compliance & Rights
In accordance with GDPR and international privacy laws, you have full control over your data. Since all operational data is stored locally, you can exercise your right to erasure at any time by clearing the app's data or uninstalling the application. Furthermore, crash logs and usage analytics are strictly opt-in and can be managed directly within the app.

## 6. Contact Information
If you have any questions regarding your privacy, please contact the developer at:<br>
**{{ site.email }}**
