# Privacy Policy for Illay Apps

**Last Updated:** April 29, 2026
**Version:** 2.0

This Privacy Policy describes how **Illay** ("we," "our," or "us") collects, uses, shares, and protects your personal information when you use the **Illay App** (Passenger) and the **Illay Driver App** (Driver) (collectively, "the Apps").

By downloading, installing, or using our Apps, you agree to the practices described in this policy. If you do not agree, please do not use the Apps.

---

## 1. Information We Collect

### 1.1 Information You Provide Directly

- **Registration Data:** Full name, email address, phone number, and optional profile picture.
- **Identity Verification (Drivers only):** National ID or driver's license number, to comply with local transportation regulations and ensure passenger safety.
- **Trip Preferences:** Pickup and drop-off locations you enter manually.

### 1.2 Location Information

Location data is essential for the Illay service to function.

- **Passengers (Foreground only):** We collect your precise GPS location while you have the App open and active. This is used to show nearby trips, estimate pickup times, and track your ride in progress. We do **not** collect passenger location in the background.

- **Drivers (Foreground and Background):** We collect your precise GPS location even when the App is in the **background** (screen off or while using another app), but **only** when you are marked as "Online" or an active trip is in progress. This is necessary to:
    - Allow passengers to track their vehicle in real-time.
    - Calculate accurate ETA (Estimated Time of Arrival).
    - Record the official route for safety auditing and legal compliance.
    - Detect unsafe speed events as part of our Safe-Drive protection system.

  Background location collection **stops automatically** when the trip ends or when the driver goes "Offline."

### 1.3 Usage and Device Information

- Device model, operating system version, and language settings.
- Unique device identifiers (Android ID / IDFA) for push notification delivery.
- Mobile network operator and connectivity type (WiFi / mobile data).
- App version and crash/diagnostic logs (for bug detection).

### 1.4 Trip and Transaction Data

- Trip history: routes taken, dates, times, and fare amounts.
- Ride status events (booked, boarded, completed, cancelled).
- Ratings and written reviews submitted between passengers and drivers.

### 1.5 Communications

- In-app notifications and messages exchanged through the platform (not SMS or external messaging apps).
- Customer support correspondence (email or in-app tickets).

---

## 2. How We Use Your Information

| Purpose | Data Used |
|---|---|
| Connect passengers with available trips | Location, registration data |
| Real-time vehicle tracking during a trip | Driver GPS location (background) |
| Calculate ETA and route display | GPS location |
| Verify driver identity | ID documents |
| Send trip alerts and push notifications | Device identifiers, trip data |
| Display ratings and build trust | Rating averages, review text |
| Detect and prevent fraud or abuse | Device identifiers, usage patterns |
| Customer support | Name, email, trip history |
| Legal and regulatory compliance | Identity data, trip records |
| Improve App performance and fix bugs | Crash logs, device info |

We do **not** use your information for automated decision-making or profiling that produces legal effects.

---

## 3. Permissions Requested

The Apps request the following device permissions:

| Permission | App | Why It Is Required |
|---|---|---|
| `ACCESS_FINE_LOCATION` (Foreground) | Passenger & Driver | Core service: show trips, track rides |
| `ACCESS_BACKGROUND_LOCATION` | Driver only | Track vehicle during active trip while app is backgrounded |
| `POST_NOTIFICATIONS` | Passenger & Driver | Trip status alerts (boarding, ETA, completion) |
| `CAMERA` (optional) | Driver | Profile photo upload |
| `READ_EXTERNAL_STORAGE` (optional) | Driver | Upload license/ID documents |
| `RECEIVE_BOOT_COMPLETED` | Driver | Restore notification listener after device restart |

You can revoke any permission at any time in your device **Settings → Apps → Illay**. Revoking location permission will prevent core features from functioning.

---

## 4. Third-Party Services and SDKs

Our Apps integrate third-party services that may independently collect and process data. We encourage you to review their privacy policies:

| Service | Provider | Purpose | Policy |
|---|---|---|---|
| Firebase Cloud Messaging (FCM) | Google LLC | Push notifications | [google.com/policies/privacy](https://policies.google.com/privacy) |
| Firebase Crashlytics | Google LLC | Crash reporting | [google.com/policies/privacy](https://policies.google.com/privacy) |
| TomTom Maps SDK | TomTom N.V. | Map tiles and routing | [tomtom.com/privacy](https://www.tomtom.com/privacy/) |
| DigitalOcean | DigitalOcean LLC | Backend hosting and database | [digitalocean.com/legal/privacy-policy](https://www.digitalocean.com/legal/privacy-policy/) |

We only partner with services that maintain adequate data protection standards.

---

## 5. Data Sharing and Disclosure

We do **not** sell your personal information to third parties. We share data only in the following circumstances:

- **Between Users During a Trip:** The driver's first name and real-time location are shared with the passenger who booked a seat on their trip. The passenger's first name and pickup point are shared with the driver.
- **Infrastructure Providers:** We use DigitalOcean (cloud hosting) and Firebase (notifications/crash reporting) to operate the service. These providers act as data processors under contractual data protection agreements.
- **Legal Requirements:** We may disclose your information when required by applicable law, court order, or in response to valid requests by government authorities. When permitted, we will notify you of such a request.
- **Safety Emergencies:** We may share information with emergency services or relevant authorities if we have reason to believe there is an imminent risk to the life or safety of any person.
- **Business Transfers:** In the event of a merger, acquisition, or sale of assets, user data may be transferred. We will notify users via a prominent in-app notice before personal data is subject to a different privacy policy.

---

## 6. International Data Transfers

Illay is headquartered in [Country — TBD]. Your data may be stored and processed in data centers located in the United States or other countries through DigitalOcean or Google Firebase. Where required by applicable law, we ensure appropriate safeguards (e.g., Standard Contractual Clauses) are in place before transferring personal data across borders.

---

## 7. Data Retention

| Data Type | Retention Period |
|---|---|
| Account profile data | Duration of account + 30 days after deletion request |
| Trip history | 3 years (regulatory compliance) |
| GPS location logs | 90 days after trip completion |
| Crash and diagnostic logs | 30 days |
| Support correspondence | 1 year after ticket closure |

After the applicable retention period, data is permanently deleted or anonymized.

---

## 8. Your Rights and Choices

Depending on your jurisdiction, you may have the right to:

- **Access:** Request a copy of the personal data we hold about you.
- **Correction:** Update inaccurate or incomplete information (available directly in the App under Profile).
- **Deletion:** Request deletion of your account and associated data. Submit your request via **Settings → Delete Account** in the App or by emailing viajaconillay@gmail.com. We will process your request within 30 days.
- **Portability:** Request your data in a machine-readable format.
- **Withdraw Consent:** You may disable location sharing at any time in device settings, though this will limit App functionality.
- **Object to Processing:** You may object to data processing based on legitimate interests by contacting us.

To exercise any of these rights, contact us at **viajaconillay@gmail.com** with the subject line "Privacy Request."

---

## 9. Security

We implement the following measures to protect your personal data:

- Data encrypted in transit (TLS 1.2+) and at rest (AES-256).
- Authentication via signed JWT tokens with short expiry and secure refresh flows.
- Role-based access control: only authorized personnel can access user data.
- Regular security audits and dependency vulnerability scanning.

No method of transmission over the internet is 100% secure. We will notify affected users and relevant authorities in the event of a data breach as required by applicable law.

---

## 10. Children's Privacy

Our Apps are **not directed to children under the age of 13** (or the applicable minimum age in your jurisdiction). We do not knowingly collect personal information from children. If you are a parent or guardian and believe your child has provided us with personal information, please contact us at **viajaconillay@gmail.com** and we will delete that information promptly.

---

## 11. Changes to This Policy

We may update this Privacy Policy from time to time. When we make material changes, we will:

1. Update the **"Last Updated"** date at the top of this page.
2. Notify you via a push notification or an in-app banner at least **7 days** before the change takes effect.
3. For significant changes affecting your rights, we may ask for renewed consent.

Continued use of the Apps after the effective date constitutes acceptance of the updated policy.

---

## 12. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy, please contact us:

- **Email:** [EMAIL_ADDRESS](viajaconillay@gmail.com)
- **Website:** [https://viajaconillay.com](https://viajaconillay.com)

We aim to respond to all inquiries within **5 business days**.
