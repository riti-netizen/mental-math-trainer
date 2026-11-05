# Mental Math Trainer

A free, local-first arithmetic dictation trainer for iPhone, iPad and desktop browsers.

## Features
- Addition, subtraction, multiplication and exact whole-number division
- 3–7 numbers per round
- Easy / medium / hard ranges
- Adjustable speaking speed and pause between numbers
- Type your final answer; optional speech recognition where supported
- Accuracy, correct-answer count and average response time
- No account, subscription, API key, database or backend

## Best way to install on iPhone (free)
This folder is a small Progressive Web App (PWA). For the iPhone's **Add to Home Screen** installation and offline caching, it must be opened from an HTTPS website. You can use free GitHub Pages:

1. Sign in to GitHub or create a free account.
2. Create a new public repository, e.g. `mental-math-trainer`.
3. Upload all files in this folder to the repository's root (not the ZIP file itself).
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish the site. Open the published `https://...github.io/...` address in **Safari** on your iPhone.
7. Tap **Share → Add to Home Screen → Add**.
8. Open it from the new Home Screen icon. After the first successful load, the app files are cached for offline use.

The app itself performs all number generation and calculations on-device. GitHub Pages is only used to deliver the static files. No arithmetic data is sent to a server.

## Desktop use
You can open `index.html` directly in a modern browser. For service-worker offline caching and installability, serve the folder over HTTPS or localhost.

## iPhone notes
- Use Safari for the best Add to Home Screen experience.
- Spoken-number playback uses the iPhone's built-in speech synthesis. Voice availability and offline voice downloads depend on iOS settings.
- Voice-answer recognition is not consistently supported by iPhone browsers. If the microphone button is unavailable, tap the microphone on the iPhone keyboard to dictate the answer into the answer field, or type it.
- If speech does not play offline, connect once to the internet and check **Settings → Accessibility → Spoken Content** / Siri & Search voice downloads, then try again.

## Customising
Edit `index.html`. Number ranges are in the `ranges` object near the top of the script.
