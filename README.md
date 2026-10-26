# J.A.R.V.I.S. Voice Only

A free, open-source personal AI assistant for Android. Say "Hey Jarvis", talk to it, chat with it,
and control a 3D hologram with your hands through the camera.

Made by Shan Akhter. First released 24 October 2026.

## What it does
- Hands-free "Hey Jarvis" wake word that runs on your phone (openWakeWord).
- Voice and text chat with AI through your own free Groq key. Optional custom voice with Fish Audio.
- 3D hologram screen with hand-tracking gestures (MediaPipe).
- Tasks, memory, tools, and a HUD-style interface.
- 24/7 mode that keeps the listener alive in the background.
- Updates install over the old app. Your data stays.

## Install and update
1. Open the Releases page of this repository and download the newest APK.
2. Install it. Allow "Install unknown apps" for your browser or file manager if Android asks.
3. After that, updates come from inside the app: Settings, About, Updates.

## Privacy
No ads, no trackers, no accounts. Chats and keys are stored on your phone; messages you send to the AI go to Groq (and spoken replies to Fish Audio if you add a key). See PRIVACY_POLICY.md.

## Legal
- Licence: Apache License 2.0 (LICENSE and NOTICE).
- Terms: TERMS_AND_CONDITIONS.md. Usage rules: USAGE_POLICY.md.
- Forks and remakes: FORK_AND_BRANDING_RULES.md. Keep the credit.
- Third-party licences: THIRD_PARTY_NOTICES.md.
- The wake-word model is non-commercial only (CC BY-NC-SA 4.0).

## Building it yourself
Upload the project zip to the repo and run the "Android build" workflow. To make updatable builds
you need your own signing key stored as GitHub secrets: KEYSTORE_BASE64, KEYSTORE_PASSWORD,
KEY_ALIAS and KEY_PASSWORD. A fork built with a different key is shown as UNOFFICIAL in the app.

## Contact
shanakhter777@gmail.com
