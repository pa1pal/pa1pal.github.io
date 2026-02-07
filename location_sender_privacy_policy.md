# Privacy Policy for Location Sender

**Last Updated:** February 2, 2025

## Introduction

Location Sender ("the App") is committed to protecting your privacy. This Privacy Policy explains how we handle data in the App.

## Data Collection

**Location Sender does NOT collect, store, transmit, or share any personal data with third parties, remote servers, or analytics services.**

### What We Access

The App requires the following permissions to function:

#### READ_CALL_LOG Permission
- **Purpose:** To display your recent phone calls within the App
- **Usage:** Call log data is read from your device and displayed in the App interface
- **Storage:** All call log data remains on your device and is never uploaded anywhere
- **Sharing:** Call log data is never shared with any third parties

### What We Store Locally

The App stores the following data **locally on your device only**:

1. **Saved Locations**
   - Location names you create
   - Place names from Google Maps
   - Addresses and coordinates
   - Google Maps links
   - **Storage:** Stored in local SQLite database
   - **Access:** Only accessible by the App on your device
   - **Deletion:** Deleted when you uninstall the App

2. **App Preferences**
   - Number of recent calls to display (10, 20, or 50)
   - **Storage:** Stored in Android DataStore on your device
   - **Deletion:** Deleted when you uninstall the App

### What We DON'T Collect

- ❌ No personal identifiable information
- ❌ No contact details or phone numbers
- ❌ No location tracking or GPS data
- ❌ No analytics or usage statistics
- ❌ No advertising identifiers
- ❌ No crash reports or diagnostics
- ❌ No cookies or tracking technologies
- ❌ No account creation or login required

## Third-Party Services

The App integrates with the following third-party services, but does NOT send your data to them:

### WhatsApp
- **Integration:** When you tap "WhatsApp" button, the App opens WhatsApp using public intents
- **Data Sent:** Only the phone number and optional pre-filled message (location link or "Hello")
- **Control:** You control what is sent when you tap "Send" in WhatsApp
- **Privacy:** Refer to [WhatsApp Privacy Policy](https://www.whatsapp.com/legal/privacy-policy)

### Google Maps
- **Integration:** When you save or share locations, the App creates Google Maps links
- **Data Sent:** Only when you manually click to open Maps or share a location
- **Control:** You control when Maps is opened
- **Privacy:** Refer to [Google Maps Privacy Policy](https://policies.google.com/privacy)

## Data Security

- All data is stored locally on your device using Android's secure storage mechanisms
- No data transmission to external servers
- No cloud sync or backup
- Data is protected by your device's security (PIN, pattern, biometric)

## Your Rights

### Access
You can view all data stored by the App within the App interface.

### Delete
You can delete saved locations individually within the App.

### Revoke Permissions
You can revoke call log permission at any time:
- Android Settings → Apps → Location Sender → Permissions → Call logs → Don't allow

Revoking permission will prevent the App from displaying recent calls but won't affect saved locations.

### Complete Data Deletion
Uninstalling the App completely removes all stored data.

## Children's Privacy

The App does not knowingly collect any information from children. The App is rated for general audiences and does not have age restrictions.

## Changes to This Policy

We may update this Privacy Policy from time to time. Any changes will be posted:
- In the App (if major changes occur)
- On this page with updated "Last Updated" date
- In the Google Play Store listing

Continued use of the App after changes constitutes acceptance of the updated policy.

## Open Source

Location Sender is committed to transparency. The source code may be made available for review to verify privacy claims.

## Contact

If you have questions about this Privacy Policy or the App's privacy practices, please contact:

- **Email:** [Your Email Address]
- **GitHub:** [Your GitHub Repository URL]

## Compliance

This App complies with:
- Google Play Store policies
- Android privacy best practices
- GDPR (General Data Protection Regulation) principles
- CCPA (California Consumer Privacy Act) principles

## Summary

**In Plain English:**
- We don't collect your data
- We don't track you
- We don't sell anything
- Everything stays on your phone
- You're in complete control

---

## Technical Details

### Permissions Breakdown

```xml
<uses-permission android:name="android.permission.READ_CALL_LOG" />
```

**READ_CALL_LOG:**
- Required for displaying recent calls
- Runtime permission (you must grant it)
- Can be revoked anytime in Android settings

### Data Storage

**SQLite Database (Room):**
- Location: `/data/data/pawan.whatsappopener/databases/`
- Content: Saved locations only
- Encryption: Android's default app data protection
- Backup: Not included in cloud backups

**DataStore Preferences:**
- Location: `/data/data/pawan.whatsappopener/datastore/`
- Content: App settings (call count preference)
- Encryption: Android's default app data protection

### Network Activity

The App has **ZERO** network activity:
- No internet permission declared
- No network requests made
- No data uploaded or downloaded
- Works completely offline

### Third-Party Libraries

The App uses standard Android libraries:
- AndroidX (Google's Android support libraries)
- Room Database (local storage)
- DataStore (local preferences)
- Jetpack Compose (UI framework)

**None of these libraries collect or transmit data.**

---

## Verification

You can verify these privacy claims by:

1. **Checking Network Activity:**
   - Use network monitoring tools (e.g., NetGuard, PCAPdroid)
   - The App makes zero network requests

2. **Reviewing Permissions:**
   - Android Settings → Apps → Location Sender → Permissions
   - Only READ_CALL_LOG is requested

3. **Inspecting Source Code:**
   - [GitHub Repository URL] (if open source)
   - Review code for data collection

4. **Using Android's Privacy Dashboard:**
   - Android 12+ Settings → Privacy → Privacy Dashboard
   - Shows when READ_CALL_LOG is accessed

---

**Questions or Concerns?**

We take privacy seriously. If you have any questions or concerns about how the App handles your data, please don't hesitate to contact us.

**Your privacy is our priority. Always.**

---

*This privacy policy is effective as of February 2, 2025 and applies to version 1.0.0 and later of Location Sender.*
