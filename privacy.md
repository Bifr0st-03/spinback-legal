# Privacy Policy for SpinBack

**Effective date:** 7 September 2026
**Last updated:** 22 October 2026
**Application:** SpinBack (Android package `com.spinback.app`)
**Provider:** Jacopo Maria Caira
**Contact:** [jacopo.caira@outlook.com](mailto:jacopo.caira@outlook.com)

## The short version

SpinBack processes your app usage information, settings, activities and spin history locally on your device. The app does not transmit this information to the developer or to third parties.

There is no account, developer-operated backend, advertising, analytics or tracking SDK. The only part of SpinBack that uses the network is Google Play’s billing library, which handles the optional supporter purchase. SpinBack’s own code sends nothing over the network.

Android may back up or transfer app data through operating-system features, depending on your device settings and the app’s backup configuration. We do not operate those services or have access to those backups.

If you contact us by email, we receive the information you choose to send so that we can respond.

## Who is responsible

SpinBack is provided by Jacopo Maria Caira.

For personal information received when you contact us, or that Google Play provides to us about purchases, Jacopo Maria Caira is the data controller. You can contact us at **[jacopo.caira@outlook.com](mailto:jacopo.caira@outlook.com)**.

The app usage information and other local app data described below are processed on your device and are not made available to us.

## What the app accesses on your device

### 1. App usage data

SpinBack uses Android’s Usage Access permission (`android.permission.PACKAGE_USAGE_STATS`) to measure foreground usage time for the apps you choose to monitor and determine when your configured limit has been reached.

You enable this access in Android’s settings, usually under **Settings → Special app access → Usage access**. You can revoke it there at any time. The exact path may vary by device.

SpinBack uses app usage information for its monitoring function. It does not read messages, posts, browsing history, keystrokes or screenshots from the apps you monitor.

Usage information is processed locally and is not transmitted to us or to third parties.

### 2. Installed apps

SpinBack queries apps with a launcher activity so that you can choose which apps to monitor. It uses a scoped `<queries>` declaration rather than the broad `QUERY_ALL_PACKAGES` permission.

The resulting app list is displayed on your device and is not transmitted.

### 3. Notifications

On Android versions that require it, SpinBack requests `android.permission.POST_NOTIFICATIONS` to send reminders when you reach your configured usage limit.

You can deny or revoke this permission. Without it, SpinBack cannot deliver those notifications.

### 4. Restart after reboot

SpinBack declares `android.permission.RECEIVE_BOOT_COMPLETED` so that it can schedule monitoring again after your device restarts.

This permission is used to resume the app’s monitoring schedule, not to transmit data.

### 5. Display over other apps (optional)

SpinBack declares `android.permission.SYSTEM_ALERT_WINDOW` for the optional **Please spin me back** mode. When that mode is on and you pass your limit, SpinBack opens its own wheel screen instead of sending a notification. Android allows an app in the background to bring itself to the foreground only with this permission.

SpinBack does not draw any window, overlay or view on top of other apps. The mode is off by default: you turn it on in the app and grant the permission in Android’s settings. Without the permission, SpinBack sends a notification instead.

This permission gives the app no access to data.

### 6. Alarms & reminders (optional)

SpinBack declares `android.permission.SCHEDULE_EXACT_ALARM` so that, if you allow it in Android’s settings, its monitoring timer runs at the moment you reach your limit instead of a little later. It is off unless you allow it, and the app works without it.

The timer never wakes your device: it runs only while you are already using it. This permission gives the app no access to data.

### 7. Network access and Google Play billing

SpinBack’s manifest includes `android.permission.INTERNET` and `com.android.vending.BILLING`. Both are added by the Google Play Billing Library, which SpinBack uses only for the optional supporter purchase described under *Purchases*.

SpinBack’s own code does not open network connections. It does not transmit your app usage information, settings, activities or spin history, through the billing library or otherwise.

The billing library communicates with the Google Play Store app on your device and, through it, with Google. According to Google, the library also logs information about its own operation, such as whether billing requests succeed and connection problems, to improve the library and provide support. Google processes that information under its own terms and privacy policy; we do not receive it.

## What the app stores

SpinBack stores the following in its private app storage:

* **Settings:** monitored apps, usage limits, quiet hours and notification preferences.
* **Wheel content:** activities, icons and selection weights.
* **Spin history:** when a spin occurred, the selected activity and your response, used to display your statistics.
* **Monitoring state:** information needed to track usage since your last break.
* **Supporter status:** whether you own the supporter purchase, so that the badge can show without a connection.

Android’s application sandbox normally prevents other apps from directly accessing this private storage.

We do not receive or maintain a server-side copy of this information.

## Android backups and device transfers

Depending on your device settings and the app’s backup configuration, Android may include some app data in a system backup or transfer it to another device.

These processes are handled by your operating system and backup provider under their own terms and privacy policies. We do not have access to those backups.

Deleting local app data or uninstalling SpinBack does not necessarily delete existing system backups. Android may restore previously backed-up data when you reinstall the app or set up another device.

To manage those copies, use your device’s backup and restore settings.

## Advertising, analytics and third-party libraries

SpinBack does not:

* create user accounts;
* request your name, email address or phone number within the app;
* transmit your app usage information, settings, activities or spin history;
* include advertising or use advertising identifiers;
* include analytics or crash-reporting SDKs, or collect telemetry about how you use the app;
* use your information for advertising profiles or cross-service tracking;
* sell, rent or share your local app data.

Monitoring the apps you select is used only to provide the usage reminders and statistics described in this policy.

SpinBack uses AndroidX components for local app functionality. It also uses two Google Play libraries: the In-App Updates library, which asks the Play Store app on your device whether a newer version exists, and the Play Billing Library, described above. It does not include third-party SDKs configured to collect or transmit your personal information.

## If you contact us

If you email **[jacopo.caira@outlook.com](mailto:jacopo.caira@outlook.com)**, we receive your email address, your message and any attachments or other information you choose to provide.

We use this information to respond, troubleshoot reported issues and manage the request. Please avoid sending sensitive information or information about other people unless necessary.

Support correspondence is handled through our email provider, Microsoft, and is subject to that provider’s applicable data-handling arrangements.

Where applicable under data protection law, we process support correspondence on the basis of our legitimate interests in assisting users and maintaining SpinBack. Where your request concerns a contractual obligation or legal requirement, the relevant contractual or legal basis may apply.

We retain correspondence only as long as reasonably necessary to handle the request and related follow-up, or to meet applicable legal obligations or establish, exercise or defend legal claims. The appropriate period depends on the nature of the request.

## Purchases

SpinBack is free, and all of its features are available without paying. It offers one optional, one-time in-app purchase, **SpinBack supporter**, which unlocks nothing and shows a thank-you badge in the app.

Purchases are processed by Google Play under Google’s terms and privacy policy. We do not receive your card number or other payment details. Google Play makes transaction information available to us in the Google Play Console, such as the order number, product, date, price and status. We use it to manage the sale and any refund, and to meet our accounting and tax obligations. Where applicable under data protection law, the basis for this processing is the performance of the purchase contract and compliance with legal obligations, and we keep it for as long as those obligations require.

On your device, SpinBack asks Google Play whether you own the supporter purchase and stores the result in its private storage. It confirms (acknowledges) new purchases with Google Play, as Google requires for every purchase. It does not send this information anywhere else.

If a purchase is refunded or revoked, Google Play stops reporting it and the badge disappears.

## Retention and deletion of local app data

Local app data remains on your device until it is deleted through the app, Android’s storage controls or uninstallation, subject to any system backup and restore features described above.

You can:

* **Clear app data:** usually under **Settings → Apps → SpinBack → Storage → Clear data** or **Clear storage**. This removes the app’s local settings, activities, history and monitoring state.
* **Uninstall SpinBack:** this removes its private local app data, subject to Android’s uninstall and data-retention options.
* **Revoke Usage Access:** this prevents SpinBack from obtaining further usage information through that permission. Revoking access does not itself delete information already stored.

We cannot remotely access or delete the app data stored on your device.

If you have contacted us by email, you may separately request deletion of your support correspondence, subject to applicable retention obligations.

## Your rights

Depending on your location and the applicable law, you may have rights to access, correct, delete or obtain a copy of your personal information, restrict its processing or object to certain processing.

For local app data that we do not receive, use the device controls described above. For personal information you have provided directly to us, such as support correspondence, contact **[jacopo.caira@outlook.com](mailto:jacopo.caira@outlook.com)**.

Where applicable, you also have the right to lodge a complaint with your local data protection authority.

## Children

SpinBack is not directed at children under 13. Any higher minimum age required by applicable law also applies.

The app does not transmit local app data to us, and we do not request age or account information within it.

If you believe a child has provided personal information to us through support correspondence, please contact us so that we can address it appropriately.

## Security

SpinBack relies on Android’s application sandbox and the security protections of your device to protect locally stored app data.

Device security also depends on factors such as operating-system updates, screen-lock settings and whether the device has been modified or compromised. No security measure can provide an absolute guarantee.

We do not operate a server that receives your local app usage data, settings, activities or spin history.

## Changes to this policy

We will update this policy when necessary to reflect changes in SpinBack or its data-handling practices. The “Last updated” date identifies the latest revision.

For material changes, we will provide an appropriate notice, such as an in-app notice or release notes, depending on the nature of the change.

If a change requires your consent under applicable law, we will request it before carrying out the relevant processing. Continued use of the app does not, by itself, constitute consent to processing that requires it.

## Contact

For privacy questions or requests:

**Jacopo Maria Caira**
**[jacopo.caira@outlook.com](mailto:jacopo.caira@outlook.com)**
