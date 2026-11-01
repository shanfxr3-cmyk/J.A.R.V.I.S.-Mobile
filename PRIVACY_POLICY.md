# Privacy Policy

J.A.R.V.I.S. Mobile
Last updated: 1 November 2026. First released: 24 October 2026.

## 1. Purpose and Scope
1.1 This Privacy Policy (the "Policy") sets out how J.A.R.V.I.S. Mobile (the "Application") handles information in connection with its use. The Application is designed, built and published by Shan Akhter, an individual developer (the "Developer", "we", "us").
1.2 This Policy applies to official builds of the Application, being builds signed with the Developer's key and published on the Releases page of the project repository.
1.3 By accepting this Policy the User acknowledges the practices described herein. Acceptance is requested again whenever this Policy, the Terms and Conditions or the Usage Policy change materially (see Section 12).

## 2. Executive Summary
- The Developer operates no servers for the Application and receives no copy of the User's conversations, voice or credentials.
- The Application contains no advertising, no analytics, no tracking technologies and no user accounts, and no information is sold or licensed to any party.
- The Application does not request the camera permission and does not read the device's location.
- Information is stored on the User's device (not on any server of the Developer) and is removed when the Application is deleted. Content sent to the third-party services in Section 4 is held by them under their own policies.
- Certain functions transmit information directly from the device to independent third-party services. These are enumerated in Section 4.

## 3. Information Stored on the Device
3.1 The Application stores the following within its private storage area on the device:
- Conversation history, limited to the most recent 500 messages;
- Task entries created by the User;
- The User's name, where supplied;
- Configuration settings, including wake-word sensitivity, voice preferences, personality choice, the User's own style instructions, a saved city name for weather, the morning-briefing schedule, the floating-bar and app-lock choices;
- Short facts the User asked the Application to remember (at most 60) and topics the User asked it to watch (at most 5);
- Third-party API credentials supplied by the User (Groq and, optionally, Fish Audio);
- A record of acceptance of the Terms and Conditions and this Policy, comprising the version of the documents accepted and the time of acceptance.
3.2 Safeguards. API credentials are encrypted before storage using AES-256-GCM, with the encryption key held in the Android Keystore. The Application disables Android backup facilities so that its data is not copied to cloud or computer backups. Conversation history and task entries are protected by the operating system's application sandbox but are not separately encrypted. On a rooted, compromised or shared device such data should be regarded as accessible.
3.3 No safeguard is absolute. The Developer does not warrant that stored information is immune from unauthorised access.

## 4. Information Transmitted to Third Parties
4.1 The following transmissions occur directly between the User's device and the named third party. The Developer is not a party to, and does not receive, these transmissions. Each third party operates under its own terms and privacy policy, which the User should review.
- Groq (api.groq.com). When the User converses with the Application, the message, recent conversation history, the current date and time, the User's name (if set), the saved city, remembered facts, watched topics, style instructions, the titles of open tasks, and the results of any tool the AI used (for example text of web pages it read, weather, battery level) are transmitted to Groq, using the User's own API credential, for the purpose of generating a response.
- Web search and page reading (DuckDuckGo, Wikipedia and the websites the AI chooses to open). When the AI needs current information it sends a short search query to DuckDuckGo or Wikipedia and may open pages on the public web, which can see the device's IP address. Pages on private or local networks are blocked. Page text is passed to Groq as described above and is treated as data, not as instructions. Sources used are listed under the reply.
- Open-Meteo (open-meteo.com). For weather, only a city name (the one the User says or saved) is sent. The device's location is never read.
- Fish Audio (api.fish.audio). Only where the User supplies a Fish Audio credential, the text of the Application's reply is transmitted for speech synthesis. Absent a credential, the device's built-in voice is used and nothing is transmitted.
- Android speech recognition. Following activation by the wake word or by manual tap, the User's speech is converted to text by the speech service installed on the device, ordinarily provided by Google. Depending on the device, language packs and settings, audio may be processed by Google. The Developer does not receive this audio.
- GitHub (github.com and api.github.com). The Application retrieves wake-word model files once from the openWakeWord project, and checks for and downloads updates from the Releases page of this project. GitHub may observe the device's IP address and the fact that a request was made.
4.2 No other transmission occurs. There is no concealed upload.
4.3 These connections use HTTPS. Third parties may process information outside the User's country of residence, and the Developer has no control over such processing.

## 5. Microphone
5.1 The wake-word detector executes locally on the device. Audio is analysed in volatile memory and discarded. It is not recorded, stored or transmitted while the Application awaits the wake word.
5.2 Upon detection of the wake word, or upon manual activation, the speech recognition described in Section 4 assumes control.
5.3 While the listener is active the operating system displays a persistent notification and a microphone indicator. This behaviour is intentional and cannot be suppressed by the Application.

## 6. Camera and Location
6.1 The Application does not request the camera permission and cannot access the camera.
6.2 The Application does not request any location permission and does not read the device's location. Weather uses only a city name that the User states or saves.

## 7. Permissions
7.1 The Application requests the following permissions, each solely for the purpose stated:
- Microphone: wake word and voice conversation.
- Internet: AI responses, optional voice synthesis, model download and update checks.
- Notifications and foreground service: display of the persistent listening notification that keeps the listener alive.
- Wake lock, battery optimisation exemption and start after restart: continuous listening where the User enables the always-on mode.
- Alarm clock: setting timers and alarms in the clock app when the User asks.
- Display over other apps (optional, granted by the User in Android settings): the floating bar shown after the wake word. The bar cannot be touched.
- Notifications: also used for the optional morning briefing and watched-topic alerts.
- Install packages: installation of an update that the User has chosen to download. Android additionally requires the User to authorise this separately.

## 7A. Phone Actions
7A.1 The AI can act only through a fixed list of tools: timers, alarms, flashlight, media volume and media keys, battery level, weather, web search, memory and watched topics. Opening the dialer, a text message or a settings page is a separate class of tool that runs only after the User taps Allow in a dialog that the AI cannot answer; these only open the phone's own app and nothing is dialled or sent without the User's further action.
7A.2 Morning briefings and watched-topic checks run without the screen open and are read-only: the AI may look things up but is given no tool that acts on the phone.
7A.3 The Application does not use the Accessibility service, does not read other apps or the screen, and does not read contacts, messages, call history or location. Becoming the default assistant lets the power or home button open the Application; it does not share screen content with it.
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
