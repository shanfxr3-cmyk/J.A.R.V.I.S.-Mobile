# 🤖 J.A.R.V.I.S. Voice Only

### The free, open-source personal AI assistant for Android — by Shan Akhter

> 🗣️ Say **"Hey Jarvis"**, talk to it, chat with it, and control a 3D hologram with your bare hands through the camera.

![Platform](https://img.shields.io/badge/platform-Android%208.0%2B-3DDC84)
![Licence](https://img.shields.io/badge/licence-Apache%202.0-blue)
![Price](https://img.shields.io/badge/price-free-brightgreen)
![No ads](https://img.shields.io/badge/ads-none-lightgrey)

Made by **Shan Akhter**. First released **24 October 2026**.

---

## ✨ Overview

J.A.R.V.I.S. Voice Only turns your Android phone into a hands-free AI assistant with a sci-fi HUD look. It waits for **"Hey Jarvis"** on the device, understands what you say, answers out loud, and keeps your chats, tasks and keys **on your phone**.

The AI itself is **[Groq](https://groq.com)** with **your own free API key**. Nothing is locked behind a subscription, and there is no account to create with the developer.

- 🆓 Free and open source (Apache License 2.0)
- 🚫 No ads, no trackers, no accounts, no servers run by the developer
- 🔑 You bring your own free Groq key (and, if you want, a Fish Audio key for a custom voice)
- 🔄 Updates install over the old app and **your data stays**
- 🛡️ Official builds are signed, and the app tells you if your copy is **OFFICIAL** or **UNOFFICIAL**

---

## 🧩 Core Features

| Feature | Description |
|---|---|
| 🎙️ **"Hey Jarvis" Wake Word** | Runs on your phone with openWakeWord. No account, no key. Wake word → beep → you speak one request → Jarvis answers → it waits again |
| 💬 **Voice and Text Chat** | **MIC** for one request, **VOICE CHAT** for a hands-free back-and-forth, or just type. A **Stop** button cancels a reply for real |
| 🧠 **Groq AI** | Default model **GPT-OSS 120B** (best quality). Switch to **GPT-OSS 20B** for faster replies and higher free limits, or type any Groq model ID |
| 🗣️ **Spoken Replies** | Uses your phone's own text-to-speech. Turn it on or off with **SPEAK** |
| 🎤 **Custom Voice (optional)** | Add a **Fish Audio** key and voice ID for a custom voice. If it fails or is blank, the phone voice is used automatically |
| 🖐️ **3D Hologram** | A 3D sphere you control by touch, or with your **bare hands** through the camera (MediaPipe hand tracking) |
| ✅ **Tasks** | Add tasks by typing or by voice: *"add a task buy milk"* |
| 🗂️ **Memory screen** | Your saved conversation history, with counts for messages, tasks and activity. Clear it any time |
| 🛠️ **Tools** | Live battery and RAM, plus shortcuts to Wi-Fi, Bluetooth, app settings, notification settings and battery saver. **Each one asks you first** |
| 🏠 **HUD Home** | AI status, system gauges, shortcuts and a recent-activity log |
| 🔋 **24/7 Mode** | Keeps "Hey Jarvis" listening with the screen off, with a watchdog that brings the listener back |
| 🔄 **In-App Updates** | **Settings → About, legal and updates → Check** |
| 🧹 **One-Tap Wipe** | **Settings → Data and privacy → Delete all app data** removes everything |

---

## 🗣️ What You Can Say

Jarvis handles these **on the phone itself** (no AI call needed). Anything else goes to the AI.

| Say | What happens |
|---|---|
| *"Add a task call the bank"* | ✅ Adds a task (also: "create task", "new task") |
| *"What are my tasks?"* / *"list tasks"* | 📋 Reads out your open tasks |
| *"What time is it?"* | 🕐 Tells you the time |
| *"What's the date?"* / *"what day is it?"* | 📅 Tells you today's date |
| *"Open settings"* / *"go to tasks"* | 🧭 Switches screen: home, chat, 3D hologram, tasks, memory, tools, settings |
| *Anything else* | 🧠 Sent to the AI as a normal question |

> 💡 Jarvis is an **assistant you talk to**, not a phone-controller. It opens its own screens and adds tasks, but it does not tap around other apps for you. The Tools screen only offers actions Android allows, and each one asks first.

---

## 📲 Install and Update

### Requirements

| Need | Details |
|---|---|
| 📱 Phone | Android **8.0 or newer** (API 26+). The official APK is built for **arm64** phones, which is almost every phone made in recent years |
| 🌐 Internet | Needed for the AI, Fish Audio, updates, and the first-time model downloads |
| 🔑 A free Groq key | Takes about a minute, see below |
| 🎙️ Google speech services | Jarvis uses Android's built-in speech recognition and text-to-speech (normally the Google app and Google Speech Services) |

### Install

1. 📦 Open the **[Releases](../../releases)** page of this repository and download the newest **APK**.
2. 📱 Open the APK to install it. If Android asks, allow **"Install unknown apps"** for your browser or file manager.
3. 📜 On first launch you see an **AUTHORISATION REQUIRED** screen. Read the key points, tick the box, and accept to continue.
4. 🔄 After that, updates come from inside the app: **Settings → About, legal and updates**.

> 💡 An update installs **over** the old app only when both APKs are signed with the **same key**. Always install official builds from this repository's Releases page.

### How updating works

- 🔎 The app checks this repository's **latest Release** when it opens (you can switch that off in the About screen).
- ⬇️ Tap **Download and install**. The app checks that the new APK is signed with the **same key** as the installed one before it hands it to Android.
- 💾 Your chats, tasks and settings stay.

---

## ⚡ Quick Start — Set Up Jarvis for Yourself

### 1️⃣ Get a free Groq API key 🔑

1. Go to **[console.groq.com](https://console.groq.com)** and sign up (free).
2. Open **API Keys** and create a new key.
3. Copy it and keep it private. It is a password.

### 2️⃣ Add the key to Jarvis ⚙️

1. Open Jarvis → bottom bar **Settings**.
2. Tap **AI provider**.
3. Paste your key into **API key**.
4. Pick a model: **GPT-OSS 120B** (default, best quality) or **GPT-OSS 20B** (faster, higher free limits).
5. Tap **Save & test**. You should see **Connected.** in green.
6. The Home screen now shows **KEY SET** and **AI READY**.

> 🔒 Your key is stored on your phone only and is sent only to `api.groq.com`.

### 3️⃣ Tell Jarvis your name 👤

**Settings → Profile** → type your name → **Save**. Jarvis uses it when it talks to you.

### 4️⃣ Turn on "Hey Jarvis" 🎙️

1. **Settings → Wake word → Turn wake word ON**.
2. Allow the **microphone** permission, and **notifications** on Android 13+.
3. The first time, a small model (about **3 MB**) downloads. This needs internet once.
4. When the status reads **WAITING**, say **"Hey Jarvis"**. You hear a beep, then speak your request.
5. Use the **Sensitivity** slider if it hears you too rarely or too often. Higher hears more, but triggers by mistake more often.

### 5️⃣ (Optional) Give Jarvis a custom voice 🎤

1. Make an account at **[fish.audio](https://fish.audio)** and create an **API key**.
2. Choose a voice there and copy its **Voice ID** from the voice page's URL.
3. In Jarvis: **Settings → Voice → FISH AUDIO (OPTIONAL)**. Paste both.
4. Pick a model: **S2.1 Pro (free)** is the default. **S2 Pro** is higher quality and uses credits.
5. Tap **Save & test**. Use **Clear** to go back to the phone's voice.

> ⚠️ Fish Audio may change or end its free tier. If it ever fails, Jarvis simply falls back to your phone's voice.

### 6️⃣ Try it out ✅

| Try this | Where |
|---|---|
| Type or speak a question | **AI** tab |
| *"Hey Jarvis, what time is it?"* | Anywhere, with the wake word on |
| Open the 3D sphere | **Home → OPEN 3D HOLOGRAM** |

---

## 🖐️ 3D Hologram and Hand Gestures

Open it from **Home → OPEN 3D HOLOGRAM**, or say *"open hologram"*.

### 👆 Touch controls

| Gesture | Action |
|---|---|
| **Drag** | Rotate (flick for momentum) |
| **Pinch** | Zoom |
| **Two fingers** | Move |
| **Double-tap** | Reset |

### 🖐️ Hand controls (camera)

Tap **START HAND TRACKING** and allow the **camera** permission.

| Your hands | Action |
|---|---|
| 🤏 **Pinch** (thumb + index) and move | Move the sphere |
| ✊ **Fist** and move | Rotate it (release to flick) |
| 🤏🤏 **Two pinches**, apart or together | Scale up or down |
| 🔍 **Scale past about 3×** | Enter the core |
| ✊✊ **Two fists for 1.5 s** | Reset |

> 💡 **Tips:** hold the phone **40–60 cm** away so both hands fit, use good lighting, and use **CAM VIEW** to see what the camera sees. **HAND CTRL** switches hand control on or off. A stats panel shows hand count, FPS, latency and confidence.
>
> The hand-tracking model is included in official builds. If it is missing, the app downloads it **once** from Google's MediaPipe storage.

---

## 🔋 24/7 Mode — Keep "Hey Jarvis" Always On

**Settings → Keep running 24/7.**

| Part | What it does |
|---|---|
| 🔔 **Always-on switch** | Keeps the listener running with the screen off. It uses a permanent notification and holds the CPU awake. Expect extra battery use |
| 🐕 **Watchdog** | Brings the listener back if Android stops it. After 3 failed starts it gives up and says so in Settings |
| 🔋 **Allow unrestricted battery** | Asks Android to stop limiting Jarvis. The card turns green when it works |
| 🚀 **Autostart / app launch settings** | Opens your phone maker's autostart page (Xiaomi, Oppo, OnePlus, Samsung, Asus, Honor and more) |
| ⚙️ **Open app settings** | Jumps to Android's settings for Jarvis |

### Poco / Xiaomi (HyperOS) checklist

1. Tap **Allow unrestricted battery**.
2. Open **Autostart** and switch Jarvis **ON**.
3. App settings → **Battery saver** → **No restrictions**.
4. In **Recents**, long-press the Jarvis card and tap the **lock**.
5. Keep **notifications** allowed.

> ℹ️ **After a phone restart**, Android does not let apps start the microphone on their own, so Jarvis cannot always restart itself. It shows a quiet **Resume** notification instead. **Tap it once** and the listener is back. If notifications are off you will not see it, so keep them allowed.

---

## 🛠️ Troubleshooting

| Problem | Fix |
|---|---|
| ❌ **"App not installed"** when updating | The new APK is signed with a different key from the installed app. Install official builds from Releases, or uninstall first (this deletes local data) |
| 🔑 **"Invalid API key (401)"** | Re-copy your Groq key with no spaces, paste it again in **Settings → AI provider**, then **Save & test** |
| 🚫 **"No API key"** | Add a free Groq key in **Settings → AI provider** |
| ⏳ **"Rate limit reached (429)"** | Jarvis already retries and falls back to the lighter model. Wait a moment or pick **GPT-OSS 20B** |
| 🔇 **Jarvis can't hear me** | Check the microphone permission, and that no other app is using the mic |
| 🙈 **Wake word never triggers** | Turn the wake word on, raise **Sensitivity**, speak clearly, and check **WAITING** shows in Settings → Wake word |
| 🛑 **"Wake word gave up after N failed starts"** | Fix the cause shown above that message, then turn the wake word **off and on** again |
| ⬇️ **Wake word stuck on DOWNLOADING** | The 3 MB model needs internet the first time. Check your connection and try again |
| 😴 **Listener keeps dying** | Follow the **24/7 checklist** above, and tap the **Resume** notification after a restart |
| 🔈 **I can't hear replies** | Make sure **SPEAK** is on and the volume is up. If you see "No text-to-speech engine installed", install **Google Speech Services** |
| 🎤 **Custom voice not used** | Fish Audio needs **both** the API key and the Voice ID. If it fails, the phone voice is used on purpose |
| 🖐️ **Hologram doesn't react to hands** | Allow the camera permission, tap **START HAND TRACKING**, make sure **HAND CTRL** is ON, and use good light |
| 🐢 **Hologram stutters** | The app switches from GPU to CPU detection by itself. **ACCEL CPU** is the smooth default |
| 🔄 **Update check fails** | GitHub limits anonymous checks. Wait a few minutes and tap **Check** again |
| 📥 **APK won't open** | Allow **Install unknown apps** for the app you downloaded it with |
| 🧹 **Start fresh** | **Settings → Data and privacy → Delete all app data** |

---

## 🔒 Privacy

- 📱 Your chats, tasks, activity and keys are stored **on your phone**. Keys are protected with the Android Keystore.
- 🚫 The developer operates **no servers** and collects **no data**. There are no ads, trackers or accounts.
- 🌐 What does leave your phone:
  - 🧠 Your messages go **straight from your phone to Groq** to get an answer.
  - 🎤 Spoken replies go to **Fish Audio** only if you add a key.
  - 🗣️ Speech recognition may be processed by **Google**.
  - 🔄 Update checks and first-time model downloads contact **GitHub** and **Google's MediaPipe storage**.
- 🧹 **Delete all app data** removes tasks, messages, activity, API keys, downloaded models and settings, and stops the listener.

See [PRIVACY_POLICY.md](PRIVACY_POLICY.md) for the full text.

> 🔑 **Never share your API keys** or commit them to a public repository. If a key leaks, revoke it and create a new one.

---

## 🏗️ Build It Yourself (Your Own Copy)

You do **not** need Android Studio. GitHub builds the APK for you. ☁️

> ⚖️ **Before you fork:** forks are welcome under the Apache License 2.0, but you must **keep the credit**, say which files you changed, and use **your own name and icon**. Read [FORK_AND_BRANDING_RULES.md](FORK_AND_BRANDING_RULES.md) first. Your build is shown as **UNOFFICIAL** in the app, which is correct and expected.

### 📁 What your repo needs

```
your-repo/
├── .github/workflows/android.yml     # the build workflow (name it anything .yml)
├── jarvis-project.zip                # the Android project (settings.gradle.kts inside)
└── (README, LICENSE, NOTICE and policy files are synced here by the workflow)
```

### 🍴 Step 0 — Fork or create your repo

1. Fork this repository, or create a new one.
2. Make sure **Actions** are enabled (**Actions** tab → enable workflows if GitHub asks).

### ✏️ Step 1 — Point the app at *your* repo

Open `app/build.gradle.kts` inside the project and change these three values. If you skip this, your app's updater will look at the **original** repository.

```kotlin
buildConfigField("String", "REPO_OWNER", "\"your-github-username\"")
buildConfigField("String", "REPO_NAME", "\"your-repo-name\"")
buildConfigField("String", "OFFICIAL_CERT_SHA256", "\"<your own key fingerprint>\"")
```

| Value | Meaning |
|---|---|
| `REPO_OWNER` / `REPO_NAME` | Where the in-app updater looks for new Releases |
| `OFFICIAL_CERT_SHA256` | The fingerprint of **your** signing key. If it matches, the About screen says **OFFICIAL BUILD** for your copy |

Get your fingerprint after Step 2:

```bash
keytool -list -v -keystore jarvis-release.jks -alias jarvis
```

Copy the **SHA256** line, remove the colons, and make it lowercase.

### 🔐 Step 2 — Create your signing key

A signing key is what lets every build **update over the previous one**. Make it once and keep it forever.

```bash
keytool -genkeypair -v -keystore jarvis-release.jks \
  -alias jarvis -keyalg RSA -keysize 2048 -validity 10000
```

Remember the **keystore password**, the **alias** (`jarvis` above) and the **key password**.

> ⚠️ **Back up `jarvis-release.jks`** somewhere safe and private. If you lose it, you can never publish an update that installs over your old app. **Never commit it to the repo.**

### 🔤 Step 3 — Convert the key to Base64

```bash
# Linux / Termux
base64 -w 0 jarvis-release.jks

# macOS
base64 -i jarvis-release.jks
```

Copy the long output.

### 🗝️ Step 4 — Add GitHub secrets

In your repo: **Settings → Secrets and variables → Actions → New repository secret**. Add all four:

| Secret | Value |
|---|---|
| `KEYSTORE_BASE64` | The Base64 text from Step 3 |
| `KEYSTORE_PASSWORD` | Your keystore password |
| `KEY_ALIAS` | Your key alias (for example `jarvis`) |
| `KEY_PASSWORD` | Your key password |

### 📤 Step 5 — Upload the project

Upload **`jarvis-project.zip`** to the **root** of the repo (**Add file → Upload files**). Put the workflow file in `.github/workflows/`.

### ▶️ Step 6 — Run the build

Go to **Actions → Android build → Run workflow**. It also runs automatically whenever `jarvis-project.zip` changes. A build takes a few minutes.

### 📦 Step 7 — Get your APK

| Situation | Result |
|---|---|
| ✅ **All four secrets set** | The APK is signed with your key and published on **Releases** as `Jarvis-Voice-Only-v<version>-build<number>.apk`. Install it over your old copy, or update from inside the app |
| ⚠️ **Secrets missing** | The APK is still built and attached to the workflow run as the **`jarvis-apk`** artifact, but it uses a throwaway debug key. It will **not** update over an installed app and is **not** published as a release |

### 🔍 What the workflow does

1. 📂 Unpacks `jarvis-project.zip` and finds `settings.gradle.kts`.
2. 🖐️ Downloads the MediaPipe **hand-tracking model** into the app's assets.
3. 🔐 Decodes your signing key from the secrets.
4. 🔨 Builds the signed **release APK** with Gradle 8.9 and JDK 17.
5. 🏷️ Names the APK with the version and build number.
6. ⬆️ Uploads it as an artifact, and publishes a Release tagged `build-<number>` (only when signed with your key).
7. 📄 Copies the licence and policy files (including this README) back to the repo root.

> 🔢 **Version numbers:** the app's version code is the GitHub run number plus 100, and the Release tag is `build-<that number>`. That is how the in-app updater knows a Release is newer.

### 🧪 Handy build switches

Set these in `gradle.properties` if you need them:

| Setting | Use |
|---|---|
| `JARVIS_MINIFY=false` | Turn off code shrinking if a release build ever crashes on launch |
| `JARVIS_ABIS=arm64-v8a,armeabi-v7a,x86_64` | Add other CPU types, for example for an emulator |
| `JARVIS_TAG_OFFSET=0` | Only change if you edit the workflow's tag format |

### 🧱 Project layout

```
app/src/main/java/com/jarvis/aiassistant/
├── MainActivity.kt        # screens and navigation
├── WakeService.kt         # the "Hey Jarvis" background listener
├── WakeWord.kt            # openWakeWord detector
├── Ai.kt                  # Groq chat (streaming, retries, fallback model)
├── Voice.kt, FishTts.kt   # speech recognition, phone voice, Fish Audio
├── HoloScreen.kt, HoloGL.kt, HandTracker.kt, Gestures.kt   # 3D hologram and hand control
├── SettingsScreen.kt, ChatScreen.kt, HomeScreen.kt, ...    # the HUD screens
├── Updater.kt, Integrity.kt                                 # in-app updates and signature checks
└── Store.kt, Secrets.kt   # on-device storage and Keystore-protected keys
```

---

## 📜 Legal

| Document | |
|---|---|
| ⚖️ **Licence** | Apache License 2.0 — [LICENSE](LICENSE) and [NOTICE](NOTICE) |
| 📋 **Terms** | [TERMS_AND_CONDITIONS.md](TERMS_AND_CONDITIONS.md) |
| ✅ **Usage rules** | [USAGE_POLICY.md](USAGE_POLICY.md) |
| 🔒 **Privacy** | [PRIVACY_POLICY.md](PRIVACY_POLICY.md) |
| 🍴 **Forks and remakes** | [FORK_AND_BRANDING_RULES.md](FORK_AND_BRANDING_RULES.md) — **keep the credit** |
| 🙏 **Third-party licences** | [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) |
| 🛡️ **Security** | [SECURITY.md](SECURITY.md) |

- 🎙️ The **"Hey Jarvis" wake-word model is non-commercial only** (CC BY-NC-SA 4.0). Do not use it in a commercial product.
- 🏷️ Not affiliated with, endorsed by, or sponsored by Marvel, Disney or any film studio. See the name notice in the branding rules.
- 📖 All of these documents are also inside the app under **Settings → About, legal and updates**.

---

## 🙏 Built With

| Piece | Used for |
|---|---|
| [openWakeWord](https://github.com/dscripka/openWakeWord) + ONNX Runtime | "Hey Jarvis" detection on the phone |
| [MediaPipe Hand Landmarker](https://ai.google.dev/edge/mediapipe) | Hand tracking for the 3D hologram |
| [Groq](https://groq.com) (your own key) | The AI that answers you |
| [Fish Audio](https://fish.audio) (optional, your own key) | A custom voice |
| Jetpack Compose + CameraX | The HUD interface and the camera |

Fonts and other credits are listed in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

---

## 🛡️ Security

Found a security problem? Please **email before posting it publicly**. See [SECURITY.md](SECURITY.md).

Official builds are **only** the APKs on this repository's Releases page, signed with the key fingerprint listed in [NOTICE](NOTICE). Do not install copies from anywhere else.

---

## 👤 Contact

Made by **Shan Akhter**.

📧 [shanakhter777@gmail.com](mailto:shanakhter777@gmail.com)

⭐ If you like J.A.R.V.I.S. Voice Only, **star the repository** to support the project!
