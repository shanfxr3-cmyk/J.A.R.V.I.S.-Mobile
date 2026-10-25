# Privacy Policy

J.A.R.V.I.S. Voice Only
Last updated: 25 October 2026. First released: 24 October 2026.

## The short version
- I don't run any servers for this app. I don't collect your data. I can't see your chats, your voice, your camera, or your keys.
- No ads. No analytics. No trackers. No accounts. No selling anything to anyone, ever.
- Your stuff lives on your phone. Delete the app and it's gone.
- Some features talk to other companies (an AI service, a voice service, GitHub). Those are listed below so there are no surprises.

## What is stored on your phone
- Your chat history (last 500 messages), your tasks, a small activity log (last 50 items).
- Your name, if you typed one in Settings.
- Your settings, and any API keys you paste in (Groq and Fish Audio).
- That you accepted these documents, and which version.
All of it sits in the app's private storage on your phone. Other apps can't read it on a normal, non-rooted phone. It is not given extra encryption by the app, so don't paste keys you can't afford to rotate on a rooted or shared phone.

## What leaves your phone, and why
- Groq (api.groq.com): when you chat or talk to Jarvis, your message goes to Groq using your own API key, together with recent chat history, the current date and time, your name if set, and the titles of your open tasks, so the AI can answer properly. Groq's own terms and privacy policy apply to that.
- Fish Audio (api.fish.audio): only if you add a Fish key. The text of Jarvis's reply is sent to turn it into speech. If you don't add a key, the phone's built-in voice is used and nothing is sent.
- Android speech recognition: after you say "Hey Jarvis", what you say next is turned into text by the speech service on your phone, normally the Google app. Depending on your phone and language packs, that audio may be processed by Google. Google's privacy policy applies to that. I don't receive it.
- GitHub (github.com, api.github.com): the app downloads the small wake-word model once from the openWakeWord project on GitHub, and checks for app updates and downloads them from this project's GitHub Releases. GitHub can see your IP address and that a request was made, like any website.
Nothing else is sent anywhere. There is no hidden upload.

## Microphone
- The "Hey Jarvis" listener runs on your phone. The audio it hears is analysed in memory on the device and thrown away. It is not recorded, saved, or sent anywhere while it waits for the wake word.
- After the wake word fires, or when you tap the mic, the speech recognition described above takes over.
- While the listener is on, Android shows a notification and a microphone indicator. That's by design.

## Camera
- The 3D hologram screen can use the camera for hand tracking. Frames are processed on the phone by Google's MediaPipe library and discarded straight away. Nothing is saved or sent.

## Permissions the app asks for, and what each is for
- Camera: hand tracking on the hologram screen.
- Microphone: wake word and voice chat.
- Internet: AI chat, optional Fish voice, wake-word model download, update checks.
- Notifications and foreground service: the "Jarvis is listening" notification that keeps the listener alive.
- Wake lock, ignore battery optimisation, and start after restart: so the listener can keep running 24/7 if you turn that mode on.
- Install packages: only to install an update you chose to download. Android also makes you allow this yourself.

## How long things are kept, and deleting them
- Everything stays until you remove it. Settings has "Delete all app data". The Memory screen can clear chat history. Uninstalling the app removes everything.
- What third parties keep (Groq, Fish Audio, Google, GitHub) is up to them. Check their policies.

## Who this is for
The app is meant for adults, 18 and over. If you're younger, ask a parent or guardian before using it. I don't knowingly collect anything from anyone, children included, because I don't collect anything.

## Your rights (India)
I'm in India, and I try to follow the Digital Personal Data Protection Act, 2023 and the Information Technology Act, 2000. Since your data stays on your device and I hold none of it, there is nothing for me to hand over, correct, or erase on my side. You control it all inside the app. If you still want to ask a question, raise a concern, or file a grievance, email the address below and I'll reply within 30 days, usually much faster.

## Changes
If this policy changes in a way that matters, the app version number goes up and you'll be asked to accept the new version before carrying on.

## Contact
shanakhter777@gmail.com
