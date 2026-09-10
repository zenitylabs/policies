---
title: AgeStash Privacy policy
description: AgeStash collects nothing. Your secrets stay on your device and in the Git repository you choose.
---

# AgeStash Privacy policy

*Last updated: September 10, 2026*

This policy covers the AgeStash iOS app. It replaces our [general privacy policy](../index.md) for the app, because AgeStash works differently from our hosted products: it has no account, no server run by Zenity Labs LLC, and nothing for us to collect.

## What we collect

Nothing.

AgeStash has no sign-up, no analytics, no advertising, and no crash reporting. Zenity Labs LLC operates no server that the app talks to, and receives no data from it. We cannot see your secrets, your usage, or the fact that you installed the app.

## Where your data lives

Your password store is a Git repository that you supply. AgeStash clones it into the app's own storage on your device and reads it there. Entries stay encrypted with age or PGP on disk, and are decrypted in memory only when you open them.

Your age keys, SSH keys, PGP keys, and any passphrases you ask the app to remember are held in the iOS keychain, marked as available only on this device while it is unlocked. The app never uploads them.

Deleting the app removes its storage. Erasing the store from Settings removes the cloned repository and its index from the device.

## Network connections the app makes

AgeStash connects to two kinds of place, and nowhere else.

**Your Git remote.** When you sync, the app contacts the Git server whose URL you entered, using the credentials or SSH key you configured. That server is yours or your provider's, and this policy does not cover how it handles your data.

**Websites referenced by your entries.** If an entry has a `url` field, opening that entry makes the app request an icon from that website so it can be shown beside the entry. The request goes to the website, not to us. That website can therefore see your IP address and infer that you keep an entry for it, in the same way that visiting it would. The icon is then cached on your device.

You can switch this off: in Settings, under General, turn on **Hide Password Images**. No icon requests are made while it is on.

## Device permissions

* **Camera**, only while you scan a QR code to import a key or a one-time password.
* **Face ID or Touch ID**, only to unlock the app when you turn that lock on.
* **Notifications**, only to show a one-time password after AutoFill so that you can copy it.

None of these send anything off your device.

## AutoFill

The AutoFill extension reads the same on-device store and fills credentials into apps and websites when you ask it to. It does not record what you filled, or where.

## Third-party code

AgeStash is built on open source libraries, listed in the app under Settings, About, Open Source Components. None of them collect analytics or track you. The library that fetches website icons is the only one that makes a network request the app would not otherwise make, and it is described above.

## Sharing and disclosure

We share nothing, because we hold nothing. There is no data for us to sell, disclose, or hand over in response to a legal request.

## Your rights

Because we hold no personal data about you, there is nothing for us to export, correct, or delete on your behalf. Your data is in your possession: on your device, and in the Git repository you control.

## Changes and questions

Changes to this policy will be published on this page and the date above updated.

Questions about this policy, or about AgeStash: https://github.com/acaloiaro/passforios/issues
