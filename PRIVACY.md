# Quinoa Privacy Policy

**Effective date:** 19 October 2026
**Applies to:** the Quinoa app for macOS, version 1.0 and later

This policy explains what information Quinoa handles, where it goes, and the choices you have. Quinoa is built so that your voice and your words stay on your Mac. Where something does leave your Mac, this policy says exactly what, why and for how long.

## 1. Who we are

Quinoa is developed and published by **Avichal** ("we", "us"), an individual developer based in India. For the purposes of India's Digital Personal Data Protection Act, 2023 ("DPDP Act") and, where it applies, the EU/UK General Data Protection Regulation ("GDPR"), we are the **Data Fiduciary / data controller** for the limited data described in Section 4.

**Contact and grievance officer:** Avichal, **jokars.v1@gmail.com**. We aim to reply within 7 days and to resolve grievances within 30 days.

## 2. The short version

- Speech recognition, cleanup, your dictionary and meeting transcripts run **entirely on your Mac**. We never receive your audio or what you dictate.
- Quinoa connects to the internet only to: download its speech model, check for updates, and, **only if you turn it on**, share anonymous word corrections.
- We do not sell, rent or share your data for advertising. There are no ads, trackers or analytics SDKs in Quinoa.

## 3. Data that stays on your Mac

Quinoa stores the following **locally**, in `~/Library/Application Support/Quinoa/` unless noted. We cannot access it.

| Data | Why | How to delete |
|---|---|---|
| Your personal dictionary (`dictionary.json`) | Corrects words the model mishears | Dictionary page, or delete the file |
| Recent dictations (`learning.json`, last 100) | Learns from the fixes you make | Delete the file |
| Meeting recordings and transcripts (`Meetings/`) | Shows you your meetings | Delete a meeting in the app (moves to Trash) |
| Shared-corrections queue (`community-pending.json`) | Holds corrections waiting to be shared, if sharing is on | Turn sharing off (clears it) |
| A correction log (`~/Library/Logs/Quinoa/corrections.log`) | Helps diagnose the correction pop-up | Delete the file |
| Settings and a random app ID (macOS preferences) | Remembers your choices | Remove Quinoa and its preferences |

Audio captured while you hold the dictation key is processed in memory and in temporary files that are replaced on each dictation. Removing Quinoa and the folders above removes all local data.

## 4. Data that leaves your Mac

### 4.1 Speech model download (everyone)
On first launch, Quinoa downloads its speech model (about 450 MB) from **Hugging Face** (huggingface.co). Like any download, Hugging Face receives your IP address and standard request information. No personal data is sent by Quinoa. See Hugging Face's privacy policy.

### 4.2 Update check (everyone)
About once a day, Quinoa asks **GitHub** (api.github.com) for the latest version number. GitHub receives your IP address and standard request information. Quinoa sends no other data. See GitHub's privacy statement.

### 4.3 Community dictionary (only if you opt in)
This is **off by default**. If you turn on **"Help improve everyone's dictionary"**, Quinoa shares, about once a week:

- pairs of a mis-heard word and its correction (for example `yarr → yaar`), and how many times you made each correction;
- a **random app ID** (generated on your Mac, not linked to your name, email, Apple ID or device serial);
- the Quinoa version.

Before anything is queued, Quinoa **filters on your Mac**. A correction is shared only if both words are short (up to two words, letters only) and the corrected word is a common lowercase word or a public brand already in Quinoa's starter packs. This means **names, company names, numbers, email addresses, links and sentences are never shared**. Your audio, your dictated text, your dictionary and your meetings are never shared. You can see everything waiting to be sent in **Settings → Community dictionary**.

The data is stored in a **Google Sheet** operated by us using Google Apps Script, so Google LLC processes it on our behalf (see Google's privacy policy). We store one row per correction pair with the number of distinct app IDs that made it. A correction is added to every Quinoa user's dictionary only if **at least 10 different people** made it **and** we have reviewed and approved it.

**Retention:** pairs made by fewer than 10 people and not seen for 90 days are deleted automatically. Approved pairs are kept while Quinoa is offered.

**Receiving approved corrections:** every copy of Quinoa downloads the approved list about once a day, whether or not you share. This sends no personal data beyond your IP address to Google.

### 4.4 Feedback and crash reports (only when you choose)
If you click **Send feedback** or agree to send a crash report, your email app opens a message to us containing the app version, macOS version and your settings and permission status. You see the message and decide whether to send it. Crash reports are technical logs generated by macOS and do not contain your dictated text. We use these emails only to fix problems, keep them for up to 12 months, and then delete them.

## 5. Legal basis

- **Community dictionary:** your **consent** (DPDP Act s.6; GDPR Art. 6(1)(a)). You can withdraw it at any time by turning the setting off. Withdrawal stops future sharing and clears the local queue; it does not affect data shared before.
- **Update checks and model download:** necessary to provide and secure the app you asked for (DPDP Act s.7 "legitimate uses"; GDPR Art. 6(1)(b)/(f)).
- **Feedback emails:** your consent and our legitimate interest in responding to you.

## 6. Your rights

Depending on where you live, you have the right to: access the data we hold about you; correct or erase it; withdraw consent; nominate another person to exercise your rights (DPDP Act); object to or restrict processing and receive a copy of your data (GDPR); and lodge a complaint with a regulator: the **Data Protection Board of India**, or your local data protection authority in the EU/UK.

**To delete what you have shared:** email **jokars.v1@gmail.com** with the 8-character ID shown in Quinoa → Settings → Community dictionary. We will remove that ID from all rows within 30 days. Because we never know who you are, we cannot find your data without this ID.

## 7. International transfers

Google, GitHub and Hugging Face may process data outside your country, including in the United States. They provide safeguards such as the EU Standard Contractual Clauses. Data transferred from India is handled in line with the DPDP Act and any restrictions notified under it.

## 8. Security

Everything Quinoa sends uses encrypted HTTPS. Community data is limited to non-identifying word pairs by design. Access to the Google Sheet is restricted to us. No system is perfectly secure, but we collect so little that there is little to lose.

## 9. Children

Quinoa is not intended for children. Under the DPDP Act a child is anyone under 18; please do not turn on community sharing if you are under 18. If you believe a child has shared data, contact us and we will delete it.

## 10. Recording meetings — your responsibility

Quinoa can record your meetings on your Mac. Laws in many places require you to tell the other participants, or get their consent, before recording a conversation. You are responsible for doing so. Quinoa keeps recordings only on your Mac.

## 11. California and other US states

We do not sell or "share" personal information as those terms are defined in the California Consumer Privacy Act, and we do not use personal information for targeted advertising.

## 12. Changes

If we change this policy, we will update the effective date above and publish the new version here. If a change materially affects the community dictionary, Quinoa will ask for your consent again before sharing.

## 13. Contact

Avichal — **jokars.v1@gmail.com**
