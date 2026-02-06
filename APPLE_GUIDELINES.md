# Apple App Store Review Guidelines

When implementing or reviewing any feature for an iOS/iPadOS app, consider ALL the rules below. Proactively identify which guidelines apply to the code/feature in question and alert about possible violations before they cause rejection.

---

## Introduction

The App Store principle: a safe experience for users, an opportunity for developers. Every app is reviewed by specialists.

### Key Points
- Apps for children: parental controls work, but you must do your part
- All viewpoints are welcome, as long as they are respectful and high-quality
- Fraud attempts (manipulating reviews, stealing data, copying apps) result in removal and expulsion from the program
- You are responsible for EVERYTHING in the app: ad networks, analytics, third-party SDKs
- Some features require specific entitlements

---

## Before Submitting

- Test for crashes and bugs
- Complete and accurate metadata
- Updated contact information
- Full access for review (demo account or demo mode)
- Active backend during review
- Explain non-obvious features and IAPs in notes
- Follow design guidelines and brand guidelines

---

## 1. Safety

### 1.1 Objectionable Content

**1.1.1** Defamatory, discriminatory, or malicious content about religion, race, sexual orientation, gender, national/ethnic origin. Political satirists are generally exempt.

**1.1.2** Realistic depictions of people/animals being killed, maimed, tortured. "Enemies" in games cannot be solely from a specific real race/culture/government.

**1.1.3** Depictions that encourage illegal use of weapons or facilitate the purchase of firearms/ammunition.

**1.1.4** Explicit sexual material or pornography. Includes "hookup" apps and apps that facilitate prostitution/human trafficking.

**1.1.5** Inflammatory religious commentary or inaccurate/misleading religious quotes.

**1.1.6** False information and misleading features (fake location trackers, etc.). "For entertainment purposes" does not override this rule. Anonymous call/SMS apps or prank apps will be rejected.

**1.1.7** Harmful concepts that capitalize on recent events (conflicts, terrorist attacks, epidemics).

### 1.2 User-Generated Content (UGC)

Apps with UGC or social networks MUST include:
- A method to filter objectionable material
- A mechanism to report offensive content with timely responses
- Ability to block abusive users
- Published contact information

Apps used primarily for pornography, Chatroulette-type experiences, objectification of real people, physical threats, or bullying will be removed without notice.

**1.2.1 Creator Content:**
Apps with "creator" content are accepted if properly moderated. Creator experiences are not native apps — they are content within the app treated as UGC.

**(a)** Creator apps must have a way to identify content that exceeds the age rating and a mechanism for age restriction via verified/declared age.

### 1.3 Kids Category

- No external links, purchase opportunities, or distractions (except in an area with a parental gate)
- Comply with privacy laws for children's data collection
- No personally identifiable information sent to third parties
- No third-party analytics (except limited cases without IDFA or identifiable information)
- Contextual third-party advertising allowed in limited cases with human review of creatives

### 1.4 Physical Harm

**1.4.1** Medical apps with inaccurate data are reviewed more strictly. Apps must disclose data/methodology. No measurement of X-rays, blood pressure, temperature, glucose, or oxygen using only device sensors.

**1.4.2** Dosage calculators must come from manufacturers, hospitals, universities, insurers, pharmacies, or approved entities, or have FDA/equivalent approval.

**1.4.3** No encouragement of tobacco/vape consumption, illegal drugs, or excessive alcohol. No sale of controlled substances (except licensed pharmacies and legal cannabis dispensaries).

**1.4.4** DUI checkpoints only those published by police. Never encourage drunk driving or reckless behavior.

**1.4.5** Apps must not incite activities (gambling, challenges) or device usage in ways that risk physical harm.

### 1.5 Developer Information

App and Support URL must include an easy way to make contact. Wallet passes must have valid contact information and a dedicated certificate.

### 1.6 Data Security

Implement appropriate security measures to protect user data against unauthorized use, disclosure, or third-party access.

### 1.7 Criminal Activity Reporting

Criminal reporting apps must involve local police and can only be offered where such involvement is active.

---

## 2. Performance

### 2.1 App Completeness

**(a)** Submissions must be final versions with complete metadata and functional URLs. No placeholder text or temporary content. Test on device. Include demo account (or demo mode with prior approval). Incomplete or crashing apps will be rejected.

**(b)** IAPs must be complete, up-to-date, visible, and functional for the reviewer.

### 2.2 Beta Testing

Demos, betas, and trials do not belong on the App Store — use TestFlight. TestFlight apps must comply with App Review Guidelines. No distribution to testers in exchange for compensation.

### 2.3 Accurate Metadata

All metadata (privacy, description, screenshots, previews) must reflect the app's core experience.

**2.3.1(a)** No hidden, dormant, or undocumented features. Every new feature must be described in Notes for Review. Misleading marketing is grounds for removal.

**2.3.1(b)** Egregious or repeated behavior is grounds for removal from the Apple Developer Program.

**2.3.2** If the app has IAPs, description/screenshots/previews must clearly indicate which items require additional purchase.

**2.3.3** Screenshots must show the app in use, not just title art, login, or splash screen.

**2.3.4** Previews can only use video screen captures from the app. May include narration and explanatory overlays.

**2.3.5** Select the most appropriate category.

**2.3.6** Answer age rating honestly.

**2.3.7** Unique name (max 30 characters). No trademarked terms, popular names, or irrelevant information in metadata. Subtitles without inappropriate content or unverifiable claims.

**2.3.8** Metadata appropriate for all ages (4+ age rating even if app is rated higher). "For Kids"/"For Children" reserved for Kids Category.

**2.3.9** You are responsible for rights to all materials. Use fictional information instead of real data.

**2.3.10** Focused on the Apple experience. No names/icons/images of other mobile platforms in the app or metadata.

**2.3.11** Pre-order apps must be complete and deliverable as submitted.

**2.3.12** "What's New" must clearly describe new features. Bug fixes can use generic description.

**2.3.13** In-app events must be accurate, happen on selected dates, and deep links must direct to the correct destination.

### 2.4 Hardware Compatibility

**2.4.1** iPhone apps must run on iPad when possible.

**2.4.2** Apps must be energy efficient. No excessive battery drain, excessive heat, or cryptocurrency mining.

**2.4.3** Apple TV apps must work without hardware beyond the Siri remote or game controllers.

**2.4.4** Apps must not suggest device restart or unrelated system settings modifications.

**2.4.5** Mac App Store: sandboxed, Xcode technologies, self-contained, no auto-launch, no root, no license screens, updates via Mac App Store, current OS.

### 2.5 Software Requirements

**2.5.1** Only public APIs, current OS. Keep updated, eliminate deprecated features. APIs for intended purposes.

**2.5.2** Self-contained apps. No reading/writing outside the container. No downloading/executing code that changes functionality (except limited educational apps).

**2.5.3** No viruses, malware, or code that damages normal operation.

**2.5.4** Background services only for intended purposes (VoIP, audio, location, etc.).

**2.5.5** Fully functional on IPv6-only networks.

**2.5.6** Web browsing must use WebKit framework.

**2.5.8** No alternative desktop/home screen environments.

**2.5.9** Do not alter standard switch functions or native UI elements.

**2.5.11 SiriKit/Shortcuts:** Only intents the app can handle. Vocabulary pertinent to the app. Resolve requests as directly as possible, no ads between request and fulfillment.

**2.5.12** CallKit/SMS Fraud Extension: only block numbers confirmed as spam.

**2.5.13** Facial recognition for auth: use LocalAuthentication, alternative method for under 13.

**2.5.14** Explicit consent and visual/audible indication when recording/logging user activity.

**2.5.15** File selection apps must include items from Files app and iCloud.

**2.5.16** Widgets, extensions, and notifications related to the app's content/functionality.

**2.5.17** Apps with Matter must use Apple framework for pairing.

**2.5.18** Ads limited to the main binary. No ads in extensions, App Clips, widgets, notifications, keyboards, watchOS. Ads appropriate to age rating. No behavioral advertising based on sensitive data. Interstitial ads must have a visible close/skip button.

---

## 3. Business

### 3.1 Payments

**3.1.1 In-App Purchase:**

- Features/functionality unlocked within the app MUST use IAP (no license keys, QR codes, crypto, etc.)
- IAPs can be used for "tips"
- Credits/coins purchased via IAP cannot expire; must have a restore mechanism
- Gifting of IAP items allowed (refund only to original purchaser)
- "Loot boxes" must disclose probabilities before purchase
- Digital gift cards redeemable for digital goods: only via IAP
- Free trial: Non-Consumable IAP Tier 0, naming "XX-day Trial", disclose duration and restrictions
- NFTs: sell via IAP, view own NFTs ok (no unlocking features), browse others' NFTs ok

**3.1.1(a) Link to Other Purchase Methods:**
- StoreKit External Purchase Link Entitlements in specific regions
- Music Streaming Services Entitlements in specific regions
- US storefront: external buttons/links allowed without entitlement

**3.1.2 Subscriptions:**

**(a) Permitted Uses:** Continuous value, minimum 7-day period, available on all devices. Examples: game levels, episodic content, multiplayer, substantial updates, media, SaaS, cloud. Subscriptions must work on all devices. No extra tasks to access paid content. Free trial via App Store Connect.

**(b) Upgrades/Downgrades:** Seamless experience, no accidental duplicate subscriptions.

**(c) Subscription Information:** Clearly describe what the user receives for the price.

**3.1.3 Other Payment Methods:**

**(a) "Reader" Apps:** Access to previously purchased content (magazines, newspapers, books, audio, music, video). Free tier account creation and management permitted.

**(b) Multiplatform:** Access to content acquired on other platforms, as long as it is also available as IAP.

**(c) Enterprise:** Apps sold directly to organizations/groups for employees/students.

**(d) Person-to-Person:** Real-time services between two individuals (tutoring, medical consultation, real estate tour, fitness). One-to-few/many must use IAP.

**(e) Goods/Services Outside the App:** Physical goods consumed outside the app must use other methods (Apple Pay, credit card).

**(f) Free Stand-alone Apps:** Free companions for paid web tools, no purchases within the app.

**(g) Advertising Management Apps:** Campaign management, no IAP required.

**3.1.4 Hardware-Specific Content:** Functionality unlocked by specific hardware ok without IAP (e.g., telescope). Optional physical products ok, but IAP must be available as an alternative.

**3.1.5 Cryptocurrencies:**
- Wallets: only by organizations
- Mining: only off-device
- Exchanges: with appropriate licensing
- ICOs: only established banks/firms
- No currency for tasks (downloading apps, social posts, etc.)

### 3.2 Other Business Models

**3.2.1 Acceptable:**
- Promote own apps (if not a mere catalog)
- Collection of third-party apps for a specific need (with robust editorial content)
- Disable access to rental content after period
- Wallet passes for payments, offers, identification
- Insurance apps: free, no IAP
- Approved nonprofits: fundraising with Apple Pay
- Individual monetary gifts (100% to recipient, unrelated to digital content)
- Financial apps submitted by the financial institution

**3.2.2 Unacceptable:**
- App Store-like interface or general interest collection
- Artificially increase impressions/clicks
- Apps primarily for displaying ads
- Fundraising for charity within the app (except approved nonprofits)
- Arbitrarily restrict who can use the app
- Manipulate user visibility/status in other services
- Binary options trading
- CFDs/derivatives without licensing
- Personal loans: disclose APR (max 36%), term, no total repayment in <=60 days
- Force users to rate/review/download other apps to access functionality

---

## 4. Design

### 4.1 Copies

**(a)** Original ideas. No copying popular apps with minimal changes.

**(b)** Impersonating other apps/services = violation of the Developer Code of Conduct.

**(c)** Do not use another developer's icon/brand/name without approval.

### 4.2 Minimum Functionality

The app must have features that elevate it beyond a repackaged website. Must provide lasting entertainment or adequate utility.

**4.2.1** ARKit: rich and integrated experiences (not just dropping a model in AR view).

**4.2.2** Must not primarily be marketing, ads, web clippings, or a link collection.

**4.2.3** App must work standalone without installing another app. Additional downloads must be disclosed.

**4.2.6** Commercial template apps will be rejected (except if submitted by the content provider). Option: single binary with "picker" model.

**4.2.7 Remote Desktop:** Only connect to user's device, local network/LAN, software running on host, no iOS/App Store-like UI.

### 4.3 Spam

**(a)** No multiple Bundle IDs for the same app. Use IAP for variations.

**(b)** Do not saturate categories with apps lacking quality/uniqueness.

### 4.4 Extensions

Follow App Extension Programming Guide. Include functionality (help, settings). No marketing/ads/IAP in extensions.

**4.4.1 Keyboard Extensions:** Provide input, method for next keyboard, functional without full network access, collection only to improve keyboard. No launching other apps. No repurposing buttons.

**4.4.2 Safari Extensions:** Current Safari version, no interference with system UI, no malicious content. Access minimum necessary websites.

### 4.5 Apple Sites and Services

**4.5.1** No scraping of Apple sites or rankings with such information.

**4.5.2 Apple Music:** MusicKit allows user-initiated playback. No monetizing access to the service. No downloading/uploading music files. Cover art only in connection with playback/playlists.

**4.5.3** No spam via Game Center, Push Notifications, etc.

**4.5.4 Push Notifications:** Must not be mandatory. No sensitive data. No promotions/direct marketing without explicit opt-in. Provide opt-out.

**4.5.5** Game Center Player IDs only per Game Center terms.

**4.5.6** Apple emoji only as Unicode characters (not on other platforms or embedded in the binary).

### 4.7 Mini Apps, Mini Games, Streaming Games, Chatbots, Plugins, Emulators

Apps may offer non-embedded software (HTML5/JS mini apps, streaming games, chatbots, plugins, retro emulators).

**4.7.1** Software must: follow privacy guidelines, include content filtering/report/block, follow Guideline 3.1 for digital goods.

**4.7.2** Do not expose native APIs without Apple permission.

**4.7.3** Do not share data/permissions with individual software without explicit consent.

**4.7.4** Provide a software index with universal links.

**4.7.5** Identify software that exceeds age rating, age restriction mechanism.

### 4.8 Login Services

Apps with social login (Facebook, Google, Twitter, LinkedIn, Amazon, WeChat) MUST offer an equivalent option that:
- Limits collection to name and email
- Allows keeping email private
- Does not collect interactions for advertising without consent

**Exceptions:** own login system, alternative marketplace, educational/enterprise app, government ID, specific third-party service client.

### 4.9 Apple Pay

Provide all material information before the sale. Follow Apple Pay Marketing Guidelines and HIG. Recurring payments must disclose: renewal term, content per period, amounts, how to cancel.

### 4.10 Monetizing Built-In Capabilities

Do not monetize hardware/OS capabilities (Push Notifications, camera, gyroscope) or Apple services (Apple Music, iCloud, Screen Time APIs).

---

## 5. Legal

### 5.1 Privacy

**5.1.1 Data Collection and Storage:**

**(i) Privacy Policies:** Required in App Store Connect and within the app. Must identify: data collected, how collected, all uses, third parties shared with, retention/deletion policies, how to revoke consent.

**(ii) Permission:** User consent for collection (even anonymous data). Paid functionality cannot depend on data access. Easy way to withdraw consent.

**(iii) Minimization:** Only data relevant to core functionality. Use out-of-process picker when possible.

**(iv) Access:** Respect permission settings. Do not manipulate/force consent. Alternatives for those who do not consent.

**(v) Account Sign-In:** If the app has no significant account-based features, allow use without login. Account creation must have account deletion. Do not require irrelevant personal information. Social login cannot be the only option if core functionality is unrelated. Social credential revocation mechanism.

**(vi)** Discovering passwords/private data = removal from the program.

**(vii)** SafariViewController visible, no tracking without consent.

**(viii)** Do not compile personal information from non-direct sources without explicit consent.

**(ix)** Apps in regulated fields (banking, healthcare, gambling, cannabis, air travel, crypto) must be submitted by a legal entity.

**(x)** Requesting basic contact information is ok if optional and does not condition features.

**5.1.2 Data Use and Sharing:**

**(i)** Do not use/transmit/share personal data without permission. Disclose sharing with third parties (including third-party AI). App Tracking Transparency required for tracking. Do not force enabling push/location/tracking to access functionality.

**(ii)** Data collected for one purpose cannot be repurposed without additional consent.

**(iii)** Do not surreptitiously build user profiles. Do not identify anonymous users.

**(iv)** Do not use Contacts/Photos to build a database for sale. Do not collect information about other installed apps.

**(v)** Do not contact people via Contacts/Photos except by explicit user initiative (individual, no Select All).

**(vi)** Data from HomeKit, HealthKit, Clinical Health Records, MovementDisorder, ClassKit, facial mapping: no use for marketing/advertising/data mining.

**(vii)** Apple Pay data: share with third parties only to facilitate/improve delivery.

**5.1.3 Health and Health Research:**

**(i)** Health/fitness/medical data cannot be used for advertising/marketing/data mining (except improving health management or research with permission).

**(ii)** Do not write false data to HealthKit. Do not store personal health information in iCloud.

**(iii)** Research with humans requires consent (nature, purpose, duration, risks, confidentiality, contact, withdrawal).

**(iv)** Independent ethics committee approval required.

**5.1.4 Kids:**

**(a)** Be careful with children's personal data. Comply with COPPA, GDPR, etc. Kids apps without third-party analytics/advertising (except limited cases per 1.3).

**(b)** Apps in Kids Category or that collect/transmit personal information from minors must have a privacy policy and comply with children's privacy laws.

**5.1.5 Location Services:**

Only when directly relevant. No use for emergency services or autonomous vehicle control (except lightweight drones). Notify and obtain consent before collecting/transmitting location data.

### 5.2 Intellectual Property

**5.2.1** No protected material without permission. Apps submitted by the IP owner/licensee.

**5.2.2** Third-party services: verify terms of use.

**5.2.3** No illegal downloading/saving of third-party media (Apple Music, YouTube, SoundCloud, Vimeo).

**5.2.4** Do not suggest/imply Apple endorsement.

**5.2.5** No confusion with Apple products/interfaces. No Apple emoji in apps. No using iTunes/Apple Music previews as entertainment.

### 5.3 Gaming, Gambling, and Lotteries

**5.3.1** Sweepstakes/contests sponsored by the app developer.

**5.3.2** Official rules in the app, Apple is not a sponsor.

**5.3.3** No IAP for credits in real money gaming.

**5.3.4** Real money gaming (sports betting, poker, casino, racing): licensing required, geo-restricted, free on the App Store.

### 5.4 VPN Apps

Use NEVPNManager API, only by organizations. Disclose collected data and usage before purchase. Do not sell/use/disclose data to third parties. Do not violate local laws. If the territory requires a VPN license, provide it in App Review Notes.

### 5.5 Mobile Device Management

MDM only for commercial enterprises, educational institutions, government agencies, or limited cases (parental control, device security). Disclose data collection/usage before purchase. Do not sell/use/disclose data to third parties.

---

## Verification Checklist

When implementing/reviewing features, verify:

- [ ] **UGC**: Has filtering, report, block, contact?
- [ ] **Privacy**: Consent obtained? Data minimized? Privacy policy updated?
- [ ] **Payments**: Using IAP where required? Subscriptions with clear info?
- [ ] **Kids**: If app can be used by children, complies with COPPA/GDPR?
- [ ] **Login**: If using social login, offers equivalent alternative?
- [ ] **Metadata**: Screenshots reflect actual app? Correct age rating?
- [ ] **Content**: No objectionable/discriminatory/violent material?
- [ ] **Performance**: No excessive battery drain? IPv6 functional?
- [ ] **Design**: App has minimum functionality? Not a mere web wrapper?
- [ ] **Location**: Permission justified? Consent obtained?
- [ ] **Health**: Accurate data? No unverifiable claims?
- [ ] **Ads**: Age-appropriate? Not in extensions/widgets? Visible close button?
- [ ] **Push**: No spam? Opt-in for marketing? Opt-out available?
- [ ] **Account**: Has account deletion if has account creation?
- [ ] **IP**: Rights to all material? No third-party branding without permission?
