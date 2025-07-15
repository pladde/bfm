# 🎶 Boss Fight Music (BFM) - *Work In Progress*

---

## 📜 Project Overview

**Boss Fight Music (BFM)** is a **Vanilla World of Warcraft AddOn** designed to elevate your gameplay by playing dynamic, customized music during boss encounters. Built with the **Turtle WoW API**, BFM aims to seamlessly detect the start and end of boss fights, transitioning your in-game audio to a thrilling combat soundtrack.

*Please note: This AddOn is currently in active development. While core detection is in place, music playback and full functionality are planned for future updates.*

---

## ✨ Current Features (Development Version)

This current development build focuses on robust boss detection and debugging within the Vanilla WoW environment.

### ➕ Implemented Functionality:

* **AddOn Load Confirmation:**
    * A chat message (`"bfm successfully loaded"`) confirms when the AddOn has loaded.
    * **Known Issue:** The current load logic (`ADDON_LOADED` AND `PLAYER_ENTERING_WORLD`) is slightly off and prevents this message from firing consistently. This will be addressed in an upcoming fix!
* **Boss Fight Detection:**
    * BFM attempts to identify when you're engaging a **boss**. A "boss" is currently defined by its `UnitClassification` (`"worldboss"`, `"boss"`) or a `UnitLevel` of `-1` (common for bosses displaying `??` as their level).
    * **Combat Start:** A chat message (`"Entering in combat against a boss"`) displays when you enter combat with a recognized boss.
    * **Combat End:** A chat message (`"leave bossfight"`) indicates when you leave a boss encounter.
* **Debugging Messages:**
    * Additional chat messages (`"DEBUG: entering combat"`) provide feedback when you generally enter combat, aiding in development.

---

## 🚀 Upcoming Features

We're excited to bring these features to BFM in future updates:

* **Music Playback Integration:** The heart of BFM – enabling the actual playback of custom or predefined music during boss fights.
* **In-Game Configuration:** User-friendly options to customize music preferences, including specific tracks for different bosses, volume control, and more.
* **Advanced Boss Detection:** Refining detection logic with specific boss unit IDs, instance-based triggers, and other criteria for even greater accuracy.
* **Bug Fixes & Optimizations:** Squashing any bugs and improving performance for a smoother experience.

---

## 📦 Installation (For Testers & Developers)

Since BFM is in active development, manual installation is required:

1.  **Download:** Grab the entire repository by downloading the ZIP file or cloning it via Git.
2.  **Extract:** Unzip the downloaded file. You'll find a folder (likely named `bfm`) containing `bfm.toc` and `bfm.lua`.
3.  **Place:** Move this `bfm` folder directly into your **World of Warcraft Vanilla** `Interface/AddOns/` directory.
    * *Example Path (may vary slightly for your specific Vanilla client like Turtle WoW):*
        `...\Interface\AddOns\bfm\`
4.  **Launch:** Start your Vanilla World of Warcraft client.
5.  **Enable AddOn:** On the character selection screen, click the "AddOns" button (bottom-left). Ensure "Boss Fight Music" is listed and **enabled**.
6.  **Test:** Log into a character and keep an eye on your chat window for the debugging messages!

---


Thank u ;-)
