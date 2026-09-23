# SpecPass 🔑✨

> A modern, zero-tracking credential forge built for websites with annoying password rules and AI-powered unique usernames.

Hosted 100% free and client-side on GitHub Pages.

## ✨ Features

- **Picky Symbol Whitelisting:** Paste the exact symbols a finicky site permits (e.g., `!@#$%`). No more rejected passwords.
- **Have I Been Pwned (HIBP) Integration:** Automatically checks your generated password against billions of leaked passwords using anonymous k-Anonymity (SHA-1 prefix hashing).
- **Time-to-Crack Visualizer:** Real-time entropy calculation estimating offline brute-force crack time.
- **AI Username Studio:** Generate thematic, clever usernames tailored to strict length and formatting constraints.
- **BYOK (Bring Your Own Key) & Privacy:** Supports Google Gemini, OpenAI, and compatible APIs. Keys are stored locally in your browser (`localStorage`) and never leave your machine.
- **Zero Dependencies:** Pure HTML, modern CSS, and vanilla JavaScript. No node modules, no build steps.

## 🚀 How to Host on GitHub Pages (in 60 Seconds)

1. Create a new public repository on GitHub named `pickypass` (or your chosen name).
2. Create a file named `index.html` and paste the code from below.
3. Commit and push the file.
4. On GitHub, go to **Settings** → **Pages** (under Code and automation).
5. Under **Branch**, select `main` (or `master`) and folder `/ (root)`, then click **Save**.
6. Wait ~30 seconds, and your site is live at `[https://<your-username>.github.io/pickypass/](https://kscheid.github.io/specpass/)`!

## 🔒 Security & Privacy

- Passwords are generated using the browser's cryptographically secure pseudo-random number generator (`window.crypto.getRandomValues`).
- When querying Have I Been Pwned, only the first 5 characters of the SHA-1 hash are sent. The full password or complete hash is never transmitted across the network.
