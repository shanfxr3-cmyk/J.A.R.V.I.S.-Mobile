# Privacy Policy

J.A.R.V.I.S. Mobile
Last updated: 4 November 2026. First released: 24 October 2026.

## 1. Purpose and Scope
1.1 This Privacy Policy (the "Policy") sets out how J.A.R.V.I.S. Mobile (the "Application") handles information in connection with its use. The Application is designed, built and published by Shan Akhter, an individual developer (the "Developer", "we", "us").
1.2 This Policy applies to official builds of the Application, being builds signed with the Developer's key and published on the Releases page of the project repository.
1.3 By accepting this Policy the User acknowledges the practices described herein. Acceptance is requested again whenever this Policy, the Terms and Conditions or the Usage Policy change materially (see Section 12).

## 2. Executive Summary
- The Developer operates no servers for the Application and receives no copy of the User's conversations, voice, location or credentials. Official builds are not pointed at any server. If the User chooses to connect a personal "hub" (Section 4A), that hub is run by the User, not by the Developer.
- The Application contains no advertising, no analytics, no tracking technologies and no user accounts, and no information is sold or licensed to any party.
- The Application does not request the camera permission. It reads the device's precise location only if the User allows it, and sends it only to the User's own hub (section 6.2).
- Information is stored on the User's device (not on any server of the Developer) and is removed when the Application is deleted. Content sent to the third-party services in Section 4 is held by them under their own policies.
- Certain functions transmit information directly from the device to independent third-party services. These are enumerated in Section 4.

## 3. Information Stored on the Device
3.1 The Application stores the following within its private storage area on the device:
- Conversation history, limited to the most recent 500 messages;
- Task entries created by the User;
- The User's name, where supplied;
- Configuration settings, including wake-word sensitivity, voice preferences, personality choice, the User's own style instructions, a saved city name for weather, the morning-briefing schedule, the floating-bar and app-lock choices;
- Short facts the User asked the Application to remember (at most 60) and topics the User asked it to watch (at most 5);
- Third-party API credentials supplied by the User (Groq, Google Gemini, Fish Audio or ElevenLabs), and the address and token of the User's own hub if one is set up;
- A record of acceptance of the Terms and Conditions and this Policy, comprising the version of the documents accepted and the time of acceptance.
3.2 Safeguards. API credentials are encrypted before storage using AES-256-GCM, with the encryption key held in the Android Keystore. The Application disables Android backup facilities so that its data is not copied to cloud or computer backups. Conversation history and task entries are protected by the operating system's application sandbox but are not separately encrypted. On a rooted, compromised or shared device such data should be regarded as accessible.
3.3 No safeguard is absolute. The Developer does not warrant that stored information is immune from unauthorised access.

## 4. Information Transmitted to Third Parties
4.1 The following transmissions occur directly between the User's device and the named third party. The Developer is not a party to, and does not receive, these transmissions. Each third party operates under its own terms and privacy policy, which the User should review.
- Groq (api.groq.com) and Google Gemini (generativelanguage.googleapis.com). When the User converses with the Application, the message, recent conversation history, the current date and time, the User's name (if set), the saved city, remembered facts, watched topics, style instructions, the titles of open tasks, and the results of any tool the AI used (for example text of web pages it read, weather, battery level) are transmitted to Groq or Google Gemini (whichever model in the User's model ladder answers), using the User's own API credential for that service, for the purpose of generating a response.
- Web search and page reading (DuckDuckGo, Wikipedia and the websites the AI chooses to open). When the AI needs current information it sends a short search query to DuckDuckGo or Wikipedia and may open pages on the public web, which can see the device's IP address. Pages on private or local networks are blocked. Page text is passed to Groq as described above and is treated as data, not as instructions. Sources used are listed under the reply.
- Open-Meteo (open-meteo.com). For weather, the Application sends only a city name. If the User allows exact location, the User's own hub may send the device's coordinates to Open-Meteo to get local weather.
- Fish Audio (api.fish.audio) or ElevenLabs (api.elevenlabs.io). Only where the User supplies a credential for one of them, the text of the Application's reply is transmitted for speech synthesis. Absent a credential, the device's built-in voice is used and nothing is transmitted.
- The calendar, notification and location tools. When the User asks, the Application reads calendar events (today and the next days), recent notifications (app, title and short text) or the approximate place name, and the result is passed to the AI service in use (Groq, or the User's hub) like any other tool result. Nothing is read in the background for the Developer, and these functions work only if the User has granted the matching permission.
- Android speech recognition. Following activation by the wake word or by manual tap, the User's speech is converted to text by the speech service installed on the device, ordinarily provided by Google. Depending on the device, language packs and settings, audio may be processed by Google. The Developer does not receive this audio.
- GitHub (github.com and api.github.com). The Application retrieves wake-word model files once from the openWakeWord project, and checks for and downloads updates from the Releases page of this project. GitHub may observe the device's IP address and the fact that a request was made.
4.2 No other transmission occurs. There is no concealed upload.

## 4A. The User's Own Hub (Optional)
4A.1 The Application can connect to a "jarvis-hub": a small server program that the User runs on a computer or hosting service of the User's choice. It is optional. Without a hub address and token in Settings, nothing in this Section happens.
4A.2 With a hub configured, the Application sends to it, over https only: AI chat requests (when the User's key is a hub token), background-job requests, watch-topic changes, TV remote results and, only if the User allows exact location, the device's precise position. It receives spoken alerts and TV commands from it.
4A.3 The hub is operated by the User. It stores its data (for example remembered facts, reminders, notes and to-dos) in files on the User's own host, and it may itself contact services such as Groq, Google Gemini, Telegram, Tavily, Open-Meteo, Google News and Cloudflare under the User's own accounts. The Developer does not receive any of this and is not responsible for the User's hub or for how its host stores data. The User should protect the hub token like a password.
4A.4 If the User has saved a Groq or Gemini key and the hub cannot be reached, the Application sends the chat request directly to Groq or Google Gemini instead.
4.3 These connections use HTTPS. Third parties may process information outside the User's country of residence, and the Developer has no control over such processing.

## 5. Microphone
5.1 The wake-word detector executes locally on the device. Audio is analysed in volatile memory and discarded. It is not recorded, stored or transmitted while the Application awaits the wake word.
5.2 Upon detection of the wake word, or upon manual activation, the speech recognition described in Section 4 assumes control.
5.3 While the listener is active the operating system displays a persistent notification and a microphone indicator. This behaviour is intentional and cannot be suppressed by the Application.

## 6. Camera and Location
6.1 The Application does not request the camera permission and cannot access the camera.
6.2 The Application asks for location permission only when the User allows it (Settings > Exact location). If allowed, it reads the device's precise position, including in the background while the always-on service runs, and sends the coordinates and accuracy only to the hub address the User configured, so the hub can give local weather and rain alerts. The User can pause sharing in Settings or revoke the permission in Android settings at any time. If the User has set a home point and left "Speak first" on, the position is also used on the phone to detect leaving and arriving home, even while sharing with the hub is paused; in that case it is not sent anywhere. The developer does not receive the location.
6.3 If the User pairs a Fire TV, the Application sends remote-control commands to the TV's address on the User's local network and stores the pairing token encrypted on the device. Nothing about the TV is sent to the developer.

## 7. Permissions
7.1 The Application requests the following permissions, each solely for the purpose stated:
- Microphone: wake word and voice conversation.
- Internet: AI responses, optional voice synthesis, model download and update checks.
- Notifications and foreground service: display of the persistent listening notification that keeps the listener alive.
- Wake lock, battery optimisation exemption and start after restart: continuous listening where the User enables the always-on mode.
- Alarm clock: setting timers and alarms in the clock app when the User asks.
- Display over other apps (optional, granted by the User in Android settings): the floating bar shown after the wake word. The bar cannot be touched.
- Notifications: also used for the optional morning briefing and watched-topic alerts.
- Calendar (read only): reading upcoming events when the User asks.
- Notification access (optional, granted by the User in Android settings): letting the "what notifications did I get" tool read recent notifications. It can be switched off in Android settings at any time.
- Location (precise, approximate and background; all optional): the approximate place name when the User asks, and, if the User allows exact location, sharing the position with the User's own hub for local rain alerts while the standby service runs.
- Install packages: installation of an update that the User has chosen to download. Android additionally requires the User to authorise this separately.

## 7A. Phone Actions
7A.1 The AI can act only through a fixed list of tools: timers, alarms, flashlight, media volume and media keys, battery level, weather, web search and page reading, memory, watched topics and background jobs, opening an installed app, reading the calendar, recent notifications and approximate location, and, if the User has set one up, the remote control of a Fire TV. Opening the dialer, a text message or a settings page is a separate class of tool that runs only after the User taps Allow in a dialog that the AI cannot answer; these only open the phone's own app and nothing is dialled or sent without the User's further action.
7A.2 Morning briefings and watched-topic checks run without the screen open and are read-only: the AI may look things up but is given no tool that acts on the phone.
7A.3 Phone control (optional). If the User turns on the Accessibility service and connects Shizuku, the Application can read the text and layout of the screen, tap, swipe, type, press system keys, take screenshots, and change phone settings, permissions and apps, only when the User asks or has switched on automatic actions. Text read from the screen is passed to the AI service in use (Groq, or the User's hub) when the AI needs it to answer. The Application does not read contacts, messages or call history in the background. Uninstalling, clearing data, installing, granting or revoking permissions, rebooting, shell commands, calls and texts always need the User's approval in chat and never run by voice. The User can switch this off at any time in Android's accessibility settings and in Shizuku. It reads notifications only if the User turns on notification access, and location only as described in section 6. Becoming the default assistant lets the power or home button open the Application.

7A.4 Proactive messages. When "Speak first" is on, the standby service reads calendar events and the battery state on the phone, and, if the User has set a home point, the phone's position, to speak heads-ups, charging reminders, leaving and arriving home notices and an evening summary. This happens on the phone only: it is not sent to the AI service or to the Developer. The home point, the learned charging hours and cached address lookups are stored in the Application's private storage and are erased with its data. With "Warn by travel time" on, the address of an upcoming calendar event is sent to the phone's own geocoding service (provided by the device maker or Google, under their terms) to estimate the distance; it can be switched off in Settings. With "Mute during events" on, the Application turns Do Not Disturb on and off through Shizuku around calendar events.
7A.4 App lock, if enabled, uses Android's own fingerprint, face or screen-lock prompt. The Application never receives biometric data.

## 8. Retention and Deletion
8.1 Information remains on the device until removed by the User. "Delete all app data" in Settings stops the wake-word listener and erases everything the Application stored on the device: conversations, tasks, name, remembered facts, watched topics, API credentials, settings, downloaded model files and cached files. The Memory screen erases conversation history. Uninstalling the Application removes all of it.
8.2 Retention by third parties is governed by their own policies.

## 9. Eligibility and Minors
9.1 The Application is intended for persons aged 18 years or older. Persons below that age may use it only with the consent and under the responsibility of a parent or legal guardian.
9.2 The Developer does not knowingly collect information from any person, including minors, because the Developer collects no information.

## 10. Rights of the User
10.1 The Developer endeavours to act consistently with the data protection laws applicable to the User.
10.2 Because the Developer holds no personal data relating to the User, there is nothing for the Developer to disclose, correct or erase. The User exercises full control over stored information within the Application.
10.3 Questions, concerns and grievances may be addressed to the contact below. The Developer will respond within thirty (30) days.

## 11. Update Integrity
11.1 An update is offered for installation only when its download address is an https address on GitHub and the downloaded package is signed with the same cryptographic key as the installed copy. Installation additionally requires the confirmation of the User through the operating system.

## 12. Acceptance; Amendments
12.1 Whenever these documents change materially, the then-current Terms and Conditions, Privacy Policy and Usage Policy are presented again. Until the User has accepted them, the Application will not open, and background functions including the wake-word listener and update checks will remain inactive. Ordinary updates that do not change the documents do not require acceptance again.
12.2 The Developer may amend this Policy at any time. The amended Policy takes effect with the Release that carries it and is subject to acceptance as described above.

## 13. Contact
shanakhter777@gmail.com
