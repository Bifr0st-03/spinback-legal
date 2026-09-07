# Privacy Policy for SpinBack

**Effective date:** 7 September 2026
**Last updated:** 7 September 2026
**Application:** SpinBack (Android package `com.spinback.app`)
**Provider:** Jacopo Maria Caira
**Contact:** jacopo.caira@outlook.com

## The short version

SpinBack does not collect your data. There is no account to create, no server
to send anything to, and no third party involved.

Everything the app measures and everything you create stays in the app's
private storage on your device. We, as the developer, never see it. It is not
uploaded, not backed up to us, not sold, not shared, and not used for
advertising or profiling.

SpinBack does not request the Android `INTERNET` permission. The app is
technically incapable of sending data anywhere, and you can verify this
yourself in the app's permission list.

## Who is responsible

Jacopo Maria Caira is the data controller for the limited purposes
described below. You can reach us at jacopo.caira@outlook.com.

Because SpinBack processes everything locally on your device and we receive no
information from it, in practice we hold no personal data about you.

## What the app accesses on your device

To do its job, SpinBack reads the following **on your device only**.

### 1. App usage data (Usage Access)

SpinBack uses Android's Usage Access permission
(`android.permission.PACKAGE_USAGE_STATS`) to measure how long the apps *you*
have chosen to monitor have been in the foreground today.

- This is the core function of the app: without it, SpinBack cannot tell when
  you have passed your own scrolling limit.
- Android does not grant this permission through a normal pop-up. You must
  enable it deliberately in **Settings → Special app access → Usage access**,
  and you can revoke it there at any time.
- SpinBack reads only the time spent in apps, and only for the apps you
  selected. It cannot see, and does not attempt to see, the content of those
  apps: no messages, no posts, no browsing history, no keystrokes, no
  screenshots.
- Usage figures are computed on the device and are used to decide whether to
  show you a notification. They are never transmitted.

### 2. The list of apps installed on your device

To let you choose which apps to monitor, SpinBack asks Android for the list of
apps that have a launcher icon. It uses a scoped `<queries>` declaration rather
than the broad `QUERY_ALL_PACKAGES` permission, so it sees launchable apps
only. This list is displayed to you and is never transmitted.

### 3. Notifications

SpinBack asks for permission to post notifications
(`android.permission.POST_NOTIFICATIONS`) because the notification *is* the
product: it is how the app tells you that you have passed your limit. If you
deny it, the app tells you plainly that it can no longer do anything useful.

### 4. Restart after reboot

SpinBack declares `android.permission.RECEIVE_BOOT_COMPLETED` so that
monitoring resumes after you restart your phone. Nothing is read or sent at
boot; the app only re-arms its own internal timer.

## What the app stores, and where

All of the following is written to SpinBack's private app storage, which other
apps cannot read:

- Your settings: the apps you monitor, your time limit, quiet hours, and
  notification preferences.
- Your wheel content: the activities you added, their icons and how often you
  want them to come up.
- Your history: the record of each spin — when it happened, which activity came
  up, and what you chose to do about it — used to show your own statistics.
- Internal monitoring state: how much time has counted since your last break.

There is no cloud copy. If Android device backup is enabled on your phone, your
operating system may include app data in the backup it makes to your own
Google account; that backup is governed by Google's terms and your device
settings, not by us, and we have no access to it.

## What we do not do

To be explicit, SpinBack does not:

- create accounts or ask for your name, email address, or phone number;
- send any data to us or to any third party;
- include advertising, advertising SDKs, or ad identifiers;
- include analytics, telemetry, or crash-reporting SDKs;
- track you across apps or websites;
- build a profile of you, or make automated decisions about you;
- sell, rent, or share your data with anyone.

SpinBack contains no third-party code that collects data. Its only libraries
are Google's AndroidX components, which run locally and perform no data
collection of their own.

## Purchases

SpinBack is currently free and contains no in-app purchases.

If a paid "Pro" version is introduced in the future, the payment will be
handled entirely by the app store (Google Play or the Apple App Store). Those
stores process the transaction under their own privacy policies. We would
receive only the aggregated, anonymous sales reporting the store provides. We
would never receive or store your payment card details.

## Data retention and deletion

Your data lives on your device for as long as you keep the app.

You are in full control of deleting it:

- **Clear app data:** Settings → Apps → SpinBack → Storage → Clear data. This
  erases your settings, wheels and history immediately.
- **Uninstall the app:** removing SpinBack deletes all of its data from your
  device.
- **Revoke usage access** at any time in Settings → Special app access → Usage
  access; SpinBack will stop measuring anything.

Because we never receive your data, there is nothing for us to delete on our
side and no deletion request you need to send us.

## Your rights

If you are in the European Economic Area or the United Kingdom, data protection
law gives you rights of access, rectification, erasure, restriction,
portability and objection regarding personal data held about you.

We do not hold personal data about you, so there is nothing for us to disclose,
correct or erase. The controls listed above give you direct and complete
control over the data on your device. You may still contact us at
[CONTACT_EMAIL] with any question, and you have the right to lodge a complaint
with your local data protection authority.

## Children

SpinBack is not directed at children and is not intended for use by anyone
under the age of 13 (or the minimum age required in your country). We do not
knowingly collect data from anyone, children included.

## Security

SpinBack relies on the security model of your device: app data is stored in
private app storage that other applications cannot access, protected by your
device's own encryption and lock screen. Since nothing is transmitted, there is
no data in transit to intercept and no server of ours that could be breached.

## Changes to this policy

If a future version of SpinBack changes how data is handled, we will update
this policy and change the "Last updated" date above before releasing that
version. Significant changes will also be described in the release notes on the
app store. Continuing to use the app after an update means you accept the
revised policy.

## Contact

Questions about this policy or about privacy in SpinBack:

**jacopo.caira@outlook.com**

