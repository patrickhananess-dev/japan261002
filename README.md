# japan261002
Japan261002 — Japanese Conversation Practice (Phone Web App)

A single-file web app for practicing spoken Japanese on your phone. One side plays the store clerk / staff, the other plays the customer. The app speaks the clerk's lines aloud, you answer out loud in Japanese, and your answer is checked against the correct one. When a round ends, the roles swap.

Note: This app is built in Korean, for Korean speakers learning Japanese. The app interface (buttons, menus, settings) and the meanings shown under each Japanese sentence are in Korean. The sentences you practice are in Japanese. You can replace the Korean meanings with English (or any language) by editing the conversation text (see "Adding your own conversations").

Live app: https://patrickhananess-dev.github.io/japan261002/

No account, no server and no installation of any program is needed. Everything runs in the browser.

Features
Role-play practice — play the customer, play the clerk, or run a swapped round after the first one.
Speak your answer — uses the browser's speech recognition (Japanese). If recognition does not work well, use "Reveal answer" and grade yourself.
Forgiving grading — similar answers count as correct (hiragana/katakana and punctuation are normalized; alternative correct phrasings are supported). The pass threshold is adjustable in Settings.
Natural voice (optional) — uses your device's Japanese voice by default. You can add your own Google Cloud Text-to-Speech API key in Settings for a more natural voice (small cost, set up by you).
Study aids — furigana toggle, hide/show Korean meaning, listening-only mode, and a review list of sentences you got wrong.
Easy to extend — add or edit conversations in plain text inside the app (see "Adding your own conversations").
Included scenarios (6)
Universal expressions (at a café)
Accommodation (hotel)
Convenience store
Restaurant
Transportation (station, bus, taxi)
Shopping
Install on your phone (Android, recommended)

The app is a web page; "installing" means adding a shortcut to your home screen.

Open Chrome on your Android phone. (Do not use an in-app browser such as the one inside a messenger app; the microphone and "Add to Home screen" may not work there.)
Go to https://patrickhananess-dev.github.io/japan261002/
Tap the ⋮ menu (top right) and choose Add to Home screen (or Install app), then confirm.
Open Japan261002 from your home screen.
When asked, allow microphone access. The page must be opened over https (the link above is).

iPhone: open the link in Safari, tap Share → Add to Home Screen. Speech recognition support on iOS is limited, so use "Reveal answer" and self-grade if the microphone does not work.

How to use
Pick a scenario on the home screen.
Choose Practice as customer (or clerk). The other side's line is spoken automatically.
Tap Speak, answer in Japanese, and see your score and the correct answer.
Continue to the end. Then use the swap option to practice the other role.
Open Settings to change grading strictness, speaking speed, voices, furigana and other options.
Adding your own conversations

Open the content screen (book icon), paste text in this format, and save. It is stored only in your phone's browser.

# Scenario title

* **Clerk**: いらっしゃいませ。
  (Korean/English meaning)

* **Customer**: 大丈夫(だいじょうぶ)です。 (또는 いいえ、大丈夫(だいじょうぶ)です。)
  (Meaning)
Start a scenario with # Title.
Each line: * **Speaker**: Japanese text, with the meaning on the next line in parentheses.
Readings: write kanji followed by its reading in parentheses, e.g. 荷物(にもつ).
Extra accepted answers: add (또는 answer1 / answer2) at the end of the line.
A stage direction can be placed first in full-width brackets, e.g. （Pointing at the screen）.

To change the built-in scenarios for everyone, edit the DEFAULT_MD text inside index.html in this repository.

Privacy
The app has no backend. Settings, your own conversations and your wrong-answer list are saved only in your phone's browser storage.
Voice recognition is handled by your browser/OS speech service.
If you enter a Google Cloud API key, it is stored only on your device and is sent only to Google's Text-to-Speech endpoint. Never commit an API key to this repository.
Troubleshooting
Microphone does not work: open the page in Chrome (not an in-app browser), check the site permission for the microphone, and make sure the address starts with https.
No Japanese voice: install a Japanese voice in your phone's text-to-speech settings, or use a Google Cloud API key in Settings.
Changes do not show after an update: reload the page (or close and reopen the home-screen shortcut).
Hosting your own copy
Fork or upload index.html to a public GitHub repository.
Settings → Pages → Deploy from a branch → main / (root) → Save.
Open https://<your-username>.github.io/<repository-name>/ after a minute or two.
License / content note

Add a license of your choice (for example MIT) for the code. The sample dialogues are short, everyday travel phrases written for practice; replace or extend them with your own content as you like.
