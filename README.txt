NUMBER TRAINER — Android home-screen web app

CONTENTS
- index.html: the app
- manifest.webmanifest: install metadata
- sw.js: offline app-shell cache
- icon.svg: home-screen icon

IMPORTANT INSTALLATION NOTES
This is a Progressive Web App (PWA), not an APK. For Chrome's "Install app" / "Add to Home screen" behavior, the files must be served from a secure HTTPS website. Opening index.html directly from a file manager may let you try the page, but installation and microphone speech recognition are not guaranteed.

EASIEST DEPLOYMENT
1. Put the four app files (index.html, manifest.webmanifest, sw.js, icon.svg) in one folder.
2. Publish that folder to a static HTTPS host you control (for example, a private GitHub Pages repository or another trusted static web host).
3. On the Samsung phone, open the HTTPS address in current Google Chrome.
4. Allow microphone access when asked.
5. Use Chrome's menu (three dots) > "Install app" or "Add to Home screen".

PRIVACY
- The app does not save audio or send recordings to an app-owned server.
- Browser speech recognition may send audio to the browser/device speech service. That processing is controlled by Android/Chrome and its speech provider; it may require internet.
- Level and score progress are session-only in this starter version; voice is not stored.

RECOGNITION
The app compares the recognized speech transcript with the displayed number. Speech recognition can mishear a correct answer, so the user may need to repeat it. It supports numeric transcripts and common English number words through 99,999.
