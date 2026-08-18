---
title: FAQ
lang: en
---

# SynoDocker FAQ

SynoDocker is an iPhone app for signing in to Synology DSM and managing containers in Container Manager.

If your question is not covered here, contact us from **Contact Us** in the app.

## Getting started

### What can SynoDocker do?

After you sign in to a Synology NAS on your network, you can:

- See every container’s status, image, and CPU / memory / network overview
- Search and filter running or stopped containers
- Open container details for stats, basic info, network, mounts, environment variables, and logs
- Start, stop, restart, or force-stop a container
- Long-press to copy logs, environment variables, mount paths, the command, gateway, IP, MAC address, and port mappings

Container details require a subscription or a lifetime purchase. The container list is available after sign-in.

### What do I need?

- An iPhone running iOS 17 or later
- A Synology NAS with **Container Manager** (or the older Docker package) installed and running
- Network access to that NAS’s DSM address (same Wi-Fi, QuickConnect, or VPN / remote access)
- A DSM account that is allowed to use Container Manager

### How do I sign in?

1. Open the app and enter your NAS address: a LAN IP, DDNS hostname, or **QuickConnect ID**
2. For an IP or hostname, choose HTTP or HTTPS and confirm the port (commonly HTTP `5000`, HTTPS `5001`)
3. For a QuickConnect ID, you do not need a port; the app resolves reachable addresses automatically
4. Enter your **DSM username and password** (not a QuickConnect account)
5. If two-factor authentication is on, enter the one-time code (you can tap **Paste** next to the field)
6. Optionally keep **Remember sign-in** enabled so you do not have to type everything next time

Enter only the hostname, IP, or QuickConnect ID—no `http://` prefix. If you include a scheme or path, the app strips it automatically.

### Does it support two-factor authentication (2FA)?

Yes. If the account requires OTP, the app asks for a verification code. If the code is wrong, expired, or missing, request a new one and try again.

### Can I use a self-signed certificate?

Yes. Many NAS units use a self-signed HTTPS certificate on the LAN, and SynoDocker can connect to those addresses. Prefer HTTP or self-signed HTTPS only on networks you trust.

## Containers and details

### Why can I see the list but need a subscription to open a container?

The list is for a quick look at what is running. Details, logs, configuration, and start/stop actions are premium features. They require a monthly plan, a yearly plan, or a lifetime purchase.

### What appears on the detail screen?

- **Runtime stats:** CPU, memory, and network
- **Basics:** container ID, image, project, CPU priority, memory limit, auto-restart, web portal
- **Network and policy:** network mode, gateway, IP, MAC, restart policy, port mappings
- **Mounts and command:** real volume paths when they can be resolved to the actual shared-folder disk, plus the start command
- **Environment variables:** each `KEY` / `VALUE` on its own
- **Recent logs:** scroll inside a fixed-height panel, with ANSI color codes stripped

You can long-press to copy gateway, IP, MAC, port mappings, mounts, and the command. Environment variables and log lines also copy on long-press, with a confirmation toast.

### Start, stop, or restart failed. What should I check?

Confirm that:

- The DSM account is allowed to control that container
- The current status allows the action (for example a stopped container cannot be stopped again)
- Container Manager is running on the NAS
- Your session is still valid; if you see a sign-in expired message, sign out and sign in again

**Force stop** is for an unresponsive container. Use it with care.

### How often does the list refresh?

In **Settings**, turn on auto-refresh and choose 3 / 5 / 10 / 30 seconds, or a custom interval from 1 to 3600 seconds. Both the list and the detail screen update on that interval. You can also pull to refresh or use **Refresh** in the top-right menu.

## Subscriptions and purchases

### What can I buy?

- **Monthly:** auto-renews every month
- **Yearly:** auto-renews every year
- **Lifetime:** a one-time purchase, yours to keep

Prices are set by the App Store. You can cancel a subscription at any time in your Apple ID subscription settings.

### How do I subscribe, restore, or cancel?

- Open **View subscription** from the container list’s top-right menu, or use the subscription section in **Settings**
- After a purchase, tap **Restore purchases** on a new device signed in with the same Apple ID
- To cancel auto-renewal, tap **Manage subscription** on the paywall, or go to iPhone **Settings → Apple ID → Subscriptions**

Apple charges your Apple ID. Subscriptions renew within 24 hours of expiry unless you turn auto-renew off.

### Why is monthly still active while yearly says “Pending”?

Monthly and yearly belong to the same subscription group. When you switch from monthly to yearly, the current monthly period usually finishes first; the yearly plan starts at the next billing date. In that case:

- Monthly stays active and will not renew as monthly
- Yearly is pending until the current period ends

Switching from yearly to monthly follows the same rule.

### Do I still need a subscription after a lifetime purchase?

No. Lifetime unlocks the same features. If you still have an auto-renewing subscription, cancel it in Apple’s subscription management so you are not billed twice.

## Connection and sign-in problems

### I see “Enter a valid Synology address” or cannot connect.

- Make sure the iPhone can reach the NAS (same network, or a working VPN / remote URL)
- Enter only the IP or hostname, with no extra path
- Match the port and HTTP / HTTPS setting to the DSM login page
- Try the same address in Safari on the iPhone
- Check the NAS firewall, auto-block, and router port forwarding

### I see “Incorrect account or password”.

Use the DSM username and password, not a QuickConnect ID or Apple ID. Check capitalization and that the account is not disabled.

### I see “Docker / Container Manager is unavailable”.

Install and start Container Manager from Package Center (on older DSM this may be named Docker). Sign in to the app again. Accounts without permission for that package also cannot list containers.

### I see that there were too many failed sign-in attempts.

DSM may have temporarily blocked the account or IP. Wait and try again, and review auto-block settings under DSM **Security**.

### I see that sign-in has expired.

This can happen after the session times out or the NAS restarts. Sign out and sign in again. With **Remember sign-in** enabled, you typically only need to do this when the saved session is no longer valid.

### Can I sign in with a QuickConnect ID?

Yes. Enter your QuickConnect ID (for example `YourNAS`) or `YourNAS.quickconnect.to` in the address field. The username and password are still your **DSM account**, not a QuickConnect account.

The app tries LAN and direct addresses first, then a QuickConnect relay if needed. Same-Wi-Fi at home is usually the most reliable. If the relay fails when you are away, use a forwarded hostname or connect to the LAN IP over VPN.

## Privacy and data

### Where are my credentials stored?

Sign-in requests go directly to the Synology address you enter. They are not sent through a SynoDocker server. If **Remember sign-in** is on, the session is stored in the on-device keychain for the next launch. Signing out clears the saved session.

### Do you collect container data?

The app talks between your iPhone and your NAS. Container lists, logs, and environment variables are not uploaded to our servers. Purchases and restores are handled by the Apple App Store.

## Still need help?

In the app, open the top-right menu on the container list, go to **About**, then tap **Contact Us**. The mail composer will include the app name and version. Please also add, if you can:

- DSM version and whether Container Manager is installed
- Whether you use HTTP or HTTPS, and whether you are on the LAN
- The exact error message (never send your password or OTP code)
