# PUCKER — Your Orange Companion

A small, responsive browser app that can be hosted free on GitHub Pages. No account or API key is required.

## Features
- Cute animated orange companion and responsive phone/desktop layout
- Rule-based chat, jokes, name/likes remembered for the current open session, and a number guessing game
- Wikipedia search summaries with links and citations to result pages (requires internet)
- Optional speech playback and browser speech recognition when supported
- Basic offline caching after the first visit (web lookups still need internet)

## Important limitations
This is **not a full generative AI model**. Its conversation brain uses simple rules, not ChatGPT-level reasoning. Wikipedia lookups are a search/summary feature, not a complete web-search AI. Voice support depends on the browser and its permissions. The app does not create a floating overlay over other apps; browsers do not permit ordinary websites to do that. No user account or cloud sync is included.

## Publish on GitHub Pages
1. Sign in to GitHub and create a new repository, for example `pucker-ai`.
2. Upload `index.html`, `manifest.json`, `sw.js`, and `README.md` to the repository root.
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose branch `main` and folder `/ (root)`, then save.
6. Wait for GitHub Pages to publish the site. Open the URL shown in Settings → Pages.

GitHub Pages uses HTTPS, which is useful for browser microphone permissions. Speech recognition availability varies by browser.

## Run locally
Double-click `index.html` to try the chat. Some browser capabilities (microphone and service worker/offline install) work only on HTTPS or localhost. Wikipedia lookups need internet access.

## Privacy
The app keeps the small amount of session memory in the current page only. Messages are not sent to an AI provider. When you request a lookup, your query is sent to Wikipedia's public API. The Web search button opens DuckDuckGo in a new tab. Do not enter private or sensitive information.
