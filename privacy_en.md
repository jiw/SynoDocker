---
title: Privacy Policy
lang: en
---

# SynoDocker Privacy Policy

**Effective date:** August 20, 2026

This Privacy Policy describes how **SynoDocker** (“the app”, “we”, “us”) handles information when you use the iPhone app SynoDocker.

SynoDocker lets you sign in to a Synology NAS (DSM) from your iPhone and view or manage containers in Container Manager. We do not operate a SynoDocker cloud account or a backend that stores your NAS credentials or container data.

If you do not agree with this policy, please do not use the app.

## 1. Who we are

SynoDocker is published under the bundle identifier `com.geekast.SynoDocker`.

To ask a privacy question, use **Contact Us** in the app (**About**), or email **lavish20210717@gmail.com**.

## 2. Summary

- Sign-in and container traffic go **from your iPhone to the NAS address you enter** (or to Synology QuickConnect, if you use a QuickConnect ID). They are **not** sent to a SynoDocker server.
- We do **not** create a user account on our side, and we do **not** sell personal information.
- If you turn on **Remember sign-in**, a session token and the NAS address you used are stored in the **on-device Keychain**. Signing out deletes that session.
- Purchases are processed by **Apple**. We do not receive your full payment card details.
- The app does not include advertising or third-party analytics SDKs.

## 3. Information we process

### 3.1 Information you provide to your NAS

When you sign in, you enter:

- NAS address (LAN IP, hostname, or QuickConnect ID)
- Port and HTTP / HTTPS (when you are not using QuickConnect)
- DSM username and password
- A one-time verification code, if two-factor authentication is enabled

This information is used only to authenticate with **your** DSM and to call Container Manager APIs. The password and OTP code are sent to the NAS as part of the sign-in request. **We do not store the password or OTP on the device or on any SynoDocker server.**

After a successful sign-in, DSM returns a session identifier (and, when provided, a Synology token). Those values are used for later API calls until you sign out or the session expires.

### 3.2 Container and NAS data

While you use the app, your iPhone may receive from the NAS:

- Container names, images, status, resource usage
- Configuration (ports, mounts, environment variables, command, network addresses)
- Container logs
- Related DSM / Container Manager metadata needed to display those screens

This data is shown on your device so you can manage containers. **It is not uploaded to us.**

### 3.3 Information stored on your iPhone

| Stored locally | Purpose | Where |
| --- | --- | --- |
| Session (NAS address, account name, DSM session id / token) | Optional “Remember sign-in” so you do not have to type everything on the next launch | iOS Keychain, this device only |
| Auto-refresh on/off and refresh interval | Settings you choose in the app | App preferences on this device |

Signing out clears the Keychain session. Uninstalling the app removes local app data in the usual iOS way.

**Demo mode** creates virtual containers only in memory. Leaving demo discards that data and restores your previous refresh settings. Demo is not written to the Keychain.

### 3.4 Clipboard

If you tap **Paste** on the OTP field, the app reads the clipboard once to fill the code. If you long-press to copy a log line, environment variable, IP address, or similar field, the app writes that text to the clipboard. Clipboard access is user-initiated and stays on the device.

### 3.5 Contact email

If you use **Contact Us**, the system Mail composer may open with the app name and version in the subject. Whatever you write and send is an email you choose to send to us. Do not include passwords or OTP codes.

### 3.6 Information we do not collect

We do not collect:

- Analytics, crash-reporting, or advertising identifiers for our own tracking
- Precise location for the app’s features
- Contacts, photos, or microphone / camera data
- A SynoDocker cloud profile or mailing-list signup inside the app

## 4. How we use information

On-device and NAS-bound information is used only to:

- Sign you in to DSM and keep the session working
- List, inspect, and control containers you are allowed to manage
- Remember sign-in and refresh preferences you chose
- Process and restore in-app purchases through Apple
- Respond if you contact us

We do not use NAS credentials or container contents for advertising.

## 5. Third parties

### 5.1 Your Synology NAS

The primary recipient of sign-in and container requests is the NAS (or relay) **you** configure. That device is operated by you or your organization. Its own privacy and security settings (HTTPS, firewall, auto-block, DSM accounts) apply.

You can allow HTTP (unencrypted) connections to a user-entered NAS address. Use HTTP or a self-signed certificate only on networks you trust.

### 5.2 Synology QuickConnect

If you sign in with a **QuickConnect ID**, the app contacts Synology QuickConnect services (for example `global.quickconnect.to`) to resolve reachable NAS addresses, and may use a Synology relay if a direct address is not available. That traffic is governed by **Synology’s** terms and privacy policy, not by a SynoDocker server.

### 5.3 Apple

Subscriptions and the lifetime purchase are sold through the **App Store** using StoreKit. Apple processes payment, Apple ID, and subscription status. We receive purchase / entitlement status needed to unlock premium features (container details and control). We do not receive your full payment card number.

Apple’s privacy policy applies to App Store accounts, receipts, and subscription management.

### 5.4 No SynoDocker backend for NAS data

We do not run a service that receives your DSM password, container logs, or environment variables.

## 6. In-app purchases

Premium features (container details, logs, configuration, and start / stop / restart) require a monthly subscription, a yearly subscription, or a lifetime purchase.

- Billing, cancellation, and refunds are handled by Apple under your Apple ID.
- Restore purchases uses the same Apple ID on the device.
- We do not store a separate paid-account password.

## 7. Data retention

- **NAS session in Keychain:** until you sign out, turn off remember-sign-in on a new sign-in, or delete the app.
- **Settings preferences:** until you change them or remove the app.
- **Demo data:** until you exit demo.
- **Email you send us:** kept only as long as needed to respond and for ordinary support records.

We cannot remotely wipe data on your NAS. To remove NAS-side logs or accounts, use DSM.

## 8. Security

- Optional remembered sessions are stored in the iOS Keychain with accessibility limited to this device after first unlock.
- We do not store the DSM password after sign-in.
- Prefer HTTPS on networks you do not fully control.
- You are responsible for DSM account permissions, NAS updates, and who can reach your NAS.

No method of transmission or storage is perfectly secure. If you believe there is a vulnerability, contact us using the details in section 12.

## 9. Children

SynoDocker is not directed at children under 13 (or the equivalent age in your country). We do not knowingly collect personal information from children. If you believe a child has provided information to us by email, contact us and we will delete it.

## 10. International use

Processing happens on your iPhone, on your NAS (and, if you use QuickConnect, on Synology’s infrastructure). If you use the app while travelling, the same local-and-NAS model applies. We do not operate a SynoDocker data centre that hosts your container data.

## 11. Changes to this policy

We may update this Privacy Policy when the app or legal requirements change. The **effective date** at the top will be revised. Continued use after an update means you accept the revised policy. Material changes will be reflected in the documentation published with the app.

## 12. Contact

- In the app: container list → menu → **About** → **Contact Us**
- Email: **lavish20210717@gmail.com**

Please do not send DSM passwords, OTP codes, or Keychain exports.

## 13. Your choices

- Do not enable **Remember sign-in** if you prefer no session on the device.
- Sign out at any time to delete the saved session.
- Manage or cancel subscriptions in iPhone **Settings → Apple ID → Subscriptions**, or via **Manage subscription** in the app.
- Stop using QuickConnect and enter a LAN IP or your own hostname if you do not want Synology’s relay involved.
- Uninstall the app to remove local SynoDocker data.
