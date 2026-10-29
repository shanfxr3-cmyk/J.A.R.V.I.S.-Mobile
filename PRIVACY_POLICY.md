# Privacy Policy

J.A.R.V.I.S. Mobile
Last updated: 29 October 2026. First released: 24 October 2026.

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
- An activity log limited to the most recent 50 entries;
- The User's name, where supplied;
- Configuration settings, including wake-word sensitivity and voice preferences;
- Third-party API credentials supplied by the User (Groq and, optionally, Fish Audio and AISStream);
- World Watch settings: the switches the User has turned on, the alert interval, any keywords, and the area (a latitude, a longitude and a radius) that the User has typed in, together with the most recent results of each feed and a list of items already reported, so that the same alert is not repeated;
- Cookies and site data placed by the web pages that the User opens in the in-app browser (Section 4); and
- A record of acceptance of the Terms and Conditions and this Policy, comprising the version of the documents accepted and the time of acceptance.
3.2 Safeguards. API credentials are encrypted before storage using AES-256-GCM, with the encryption key held in the Android Keystore. The Application disables Android backup facilities so that its data is not copied to cloud or computer backups. Conversation history, task entries and World Watch settings (including the typed area) are protected by the operating system's application sandbox but are not separately encrypted. On a rooted, compromised or shared device such data should be regarded as accessible.
3.3 No safeguard is absolute. The Developer does not warrant that stored information is immune from unauthorised access.

## 4. Information Transmitted to Third Parties
4.1 The following transmissions occur directly between the User's device and the named third party. The Developer is not a party to, and does not receive, these transmissions. Each third party operates under its own terms and privacy policy, which the User should review.
- Groq (api.groq.com). When the User converses with the Application, the message, recent conversation history, the current date and time, the User's name (if set) and the titles of open tasks are transmitted to Groq, using the User's own API credential, for the purpose of generating a response.
- Fish Audio (api.fish.audio). Only where the User supplies a Fish Audio credential, the text of the Application's reply is transmitted for speech synthesis. Absent a credential, the device's built-in voice is used and nothing is transmitted.
- Android speech recognition. Following activation by the wake word or by manual tap, the User's speech is converted to text by the speech service installed on the device, ordinarily provided by Google. Depending on the device, language packs and settings, audio may be processed by Google. The Developer does not receive this audio.
- GitHub (github.com and api.github.com). The Application retrieves wake-word model files once from the openWakeWord project, and checks for and downloads updates from the Releases page of this project. GitHub may observe the device's IP address and the fact that a request was made.
4.2 World Watch. Only for the feeds that the User has switched on or opened, the Application contacts the following providers directly. Every provider can observe the device's IP address and the time of the request.
- U.S. Geological Survey (earthquake.usgs.gov): earthquake lists. Nothing about the User is sent.
- GDACS (www.gdacs.org): global disaster alerts. Nothing about the User is sent.
- U.S. National Weather Service (api.weather.gov): severe weather alerts. Nothing about the User is sent; filtering by area happens on the device.
- GDELT Project (api.gdeltproject.org): news search. The keywords entered by the User are sent.
- Where The ISS At (api.wheretheiss.at): the position of the International Space Station. Nothing about the User is sent.
- adsb.lol (api.adsb.lol): lists of aircraft. The lists are retrieved in full and filtered against the User's area on the device, so the area is not sent.
- AISStream (stream.aisstream.io): ships. Only when the User requests it, the User's own AISStream credential and the bounding box of the User's typed area are sent.
- Windy (embed.windy.com): the wind map. The latitude and longitude of the User's typed area are part of the address that is loaded.
- Live-camera, LiveATC and similar pages. A page that the User opens is loaded inside the Application and is operated by its own publisher, who may set cookies and observe the device's IP address and what the User views. Only https pages are opened, and links that would leave the Application are blocked.
4.3 No other transmission occurs. There is no concealed upload.
4.4 These connections use HTTPS (or its WebSocket equivalent). Third parties may process information outside the User's country of residence, and the Developer has no control over such processing.

## 5. Microphone
5.1 The wake-word detector executes locally on the device. Audio is analysed in volatile memory and discarded. It is not recorded, stored or transmitted while the Application awaits the wake word.
5.2 Upon detection of the wake word, or upon manual activation, the speech recognition described in Section 4 assumes control.
5.3 While the listener is active the operating system displays a persistent notification and a microphone indicator. This behaviour is intentional and cannot be suppressed by the Application.

## 6. Camera and Location
6.1 The Application does not request the camera permission and cannot access the camera. Live-camera pages shown in World Watch are third-party web pages and are not connected to the device's own camera.
6.2 The Application does not request any location permission and does not read the device's location. The area used by World Watch is only what the User types in.

## 7. Permissions
7.1 The Application requests the following permissions, each solely for the purpose stated:
- Microphone: wake word and voice conversation.
- Internet: AI responses, optional voice synthesis, World Watch feeds, model download and update checks.
- Notifications and foreground service: display of the persistent listening notification that keeps the listener alive, and of World Watch alerts where the User enables them.
- Wake lock, battery optimisation exemption and start after restart: continuous listening where the User enables the always-on mode, and the resumption of World Watch alerts after a restart.
- Install packages: installation of an update that the User has chosen to download. Android additionally requires the User to authorise this separately.

## 8. Retention and Deletion
8.1 Information remains on the device until removed by the User. "Delete all app data" in Settings stops the wake-word listener, cancels World Watch alerts and erases everything the Application stored on the device: conversations, tasks, activity, name, API credentials, World Watch settings and results, in-app browser cookies and site data, settings, downloaded model files and cached files. The Memory screen erases conversation history. Uninstalling the Application removes all of it.
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
12.1 Whenever these documents change materially, the then-current Terms and Conditions, Privacy Policy and Usage Policy are presented again. Until the User has accepted them, the Application will not open, and background functions including the wake-word listener, World Watch alerts and update checks will remain inactive. Ordinary updates that do not change the documents do not require acceptance again.
12.2 The Developer may amend this Policy at any time. The amended Policy takes effect with the Release that carries it and is subject to acceptance as described above.

## 13. Contact
shanakhter777@gmail.com
