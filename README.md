# 💌 Special Mission & Proposal Web App

An interactive, mobile-optimized proposal web app with a mini-game, evasive "No" button sequence, post-YES questionnaire wizard, celebratory effects, and instant answer tracking!

---

## 🌟 Features Included

1. **📱 Ultra-Responsive Touch Mini-Game**:
   - Tap 10 glowing hearts with countdown rings before they vanish.
   - Generous touch hitbox designed specifically for mobile fingers with zero lag.
   - Combos, lives system, sound effects (synthesized via Web Audio API, no external downloads needed).

2. **🔪 Threatening & Evasive "No" Button**:
   - **1st Tap**: Turns into `🔪 Wait what?!`, jumps to random spot, knife audio.
   - **2nd Tap**: Turns into `☠️ Don't you dare!!`, screen shakes violently.
   - **3rd Tap**: Turns into `💀 NO CHOICE!`, red flash, button disintegrates completely!
   - `YES!` button expands and pulses enticingly as the only choice left.

3. **📝 Multi-Step Post-YES Questionnaire**:
   - **Q1: Where do you wanna go?**
     - 🎬 *Movie Date* → Custom text input for movie title.
     - ✈️ *Abroad Trip* → Bali / Diamond Beach / Blue Lagoon / Custom input.
     - 🏍️ *Bike Ride* → Manali / Goa / Ladakh / Custom input.
     - ✨ *Something Else* → Custom text input.
   - **Q2: When do you wanna go?**
     - 🎒 After school / 🎓 After college / 💍 After marriage / 💀 After dead 🥲
   - **Q3: With whom do you wanna go?**
     - 💖 Only with me 😁😋 / 🙄 Group trip with your friends / 👻 After dead 🙂
   - **Official Date Boarding Pass**: Shows her summary choices + optional sweet note.

4. **🎉 Grand Celebration & Answer Sharing**:
   - Confetti cannons & floating heart balloons.
   - Direct **WhatsApp Share button** pre-filled with her chosen answers.
   - **Local Storage + Webhook Integration** so you can view what she entered.

---

## 🚀 How to Host on GitHub Pages (Free in 2 Minutes)

1. Create a new GitHub repository (e.g. `special-mission` or `for-you`).
2. Upload `index.html` to the repository root.
3. In your GitHub repository:
   - Go to **Settings** ➔ **Pages** (on the left menu).
   - Under **Build and deployment** ➔ **Branch**, select `main` (or `master`) and folder `/ (root)`.
   - Click **Save**.
4. GitHub will give you a live link (e.g. `https://yourusername.github.io/special-mission/`). Send this link to her!

---

## 📬 How to Receive Her Answers via Email (Optional Formspree Setup)

If you want her answers sent directly to your email the second she hits submit:

1. Go to [https://formspree.io](https://formspree.io) and create a free account.
2. Click **+ New Form**, name it `Proposal Responses`, and copy your Form URL (e.g., `https://formspree.io/f/mqkvyxyz`).
3. Open `index.html`, find line ~450:
   ```javascript
   const FORM_ENDPOINT = "https://formspree.io/f/YOUR_FORM_ID_HERE";
   ```
4. Paste your Formspree URL inside the quotes and save!

> **Note**: Even without Formspree, her answers are automatically formatted into a WhatsApp message link when she reaches the end, and saved in the browser's `localStorage`!
