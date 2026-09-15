# Max Vilchevskiy

**Senior iOS Engineer | AI-Enabled Software Development**

Kyiv, Ukraine · Remote

[vil4max@gmail.com](mailto:vil4max@gmail.com) · [Telegram](https://t.me/vil4max) · [LinkedIn](https://www.linkedin.com/in/vil4max/) · [Portfolio](https://vil4max.github.io)

[Resume PDF](https://vil4max.github.io/assets/Vilchevskiy_Senior_iOS_Engineer.pdf) · [Full resume](https://vil4max.github.io/full-resume.html)

## About

I'm a Senior iOS Engineer with 13 years of experience in iOS, consumer products, and fintech. I've built apps from scratch and worked on established products through years of growth. At Drinkit, I was part of the team that launched the app with its first coffee shop. At Umico, I developed marketplace features as the product grew into Birmarket, then built a subscription SDK for several host apps. My recent work also includes a watchOS voice client with an iPhone relay.

I use coding agents for planning, implementation, testing, verification, and code review in released products and R&D work. I make the technical decisions and check the results. I built and released DriveCheckUA and OneCart Family this way. DriveCheckUA includes a Foundation Models summary with structured output, validation, and deterministic fallback. I also built a separate Swift agent/tool runtime with a 38-case evaluation corpus and validation on a real device.

I'm looking for Senior iOS Engineer roles on long-term products, particularly in iOS and fintech. I can take a feature from technical planning through implementation and release, and I'd like to contribute to other parts of the product over time. AI-enabled development is part of how I work day to day.

## Technical focus

**iOS & Apple Platforms:** Swift · Objective-C · UIKit · SwiftUI · Foundation · iOS SDK · Xcode · Swift Concurrency · Combine · Auto Layout · URLSession · REST APIs · WebSockets · Core Data · Keychain Services · StoreKit 2 · watchOS · WatchConnectivity · Realtime Audio Streaming

**Architecture & Delivery:** Swift Package Manager (SPM) · Modular Architecture · MVVM · Clean Architecture · Dependency Injection · Protocol-Oriented Programming · XCTest · Xcode Instruments · Performance Optimization · CI/CD · App Store Connect

**AI Engineering & Development:** Apple Foundation Models · Context Engineering · Agentic SDLC · Agentic Workflows · Tool Calling · Structured Outputs · Continuous Evaluation · Deterministic Verification · Human-in-the-Loop Engineering · AI-Assisted Development

## Selected work

### [GlobalLogic](https://vil4max.github.io/projects.html#project-watch-ai-assistant)

An R&D Apple Watch voice assistant for hands-free fieldwork. Worked with the wider R&D team on the Apple platform client. Led watchOS interaction flows, audio streaming, and the iPhone relay. Shipped a TestFlight demo, codebase, and documentation for client evaluation.

- Built the watchOS conversation interface, translating structured assistant responses into concrete device actions and haptics.
- Implemented the companion iPhone relay for live audio and realtime WebSocket communication within watchOS runtime limits.

**Skills:** WatchKit · Swift Concurrency · WatchConnectivity · WebSockets · AVFoundation · Structured AI Responses

### [PASHA Holding](https://vil4max.github.io/projects.html#project-birmarket)

Birmarket (formerly Umico) is a consumer marketplace in the PASHA ecosystem. Embedded in the loyalty engineering team alongside backend and QA specialists. Shipped core loyalty features and spearheaded subscription modularization. Delivered a unified Swift package powering subscriptions across Birmarket, Birbank, and m10.

- Shipped high-traffic marketplace features while untangling monolithic dependencies into modular Swift packages.
- Built the multi-host Subscription SDK with an independent PostHog analytics layer, defining clean contracts for host apps.

**Skills:** UIKit · SwiftUI · Swift Concurrency · SPM · Multi-host SDK · Unit Testing · Integration Testing · CI/CD · A/B Testing · Feature Flags · Remote Configuration · PostHog

### [Drinkit](https://vil4max.github.io/projects.html#project-drinkit)

Drinkit was a digital coffee-shop startup in Dodo Brands, linking mobile ordering with preparation and pickup. Worked in a product team of about 20 across engineering, design, QA and product. Helped establish the mobile team and took ownership of iOS features and releases. Launched the app with the first coffee shop and developed the product for two years.

- Implemented drink customization and pricing, refined UX with the designer, and worked with A/B tests and feature flags.
- Built looping menu videos and offline caching, and integrated the payment SDK on the host side.

**Skills:** Swift · UIKit · Combine · SPM · GCD · OperationQueue · MVP · AVFoundation · Offline Caching · Payment SDKs · A/B Testing · Feature Flags · Remote Configuration

## Personal projects

### DriveCheckUA

DriveCheckUA helps drivers check regional safety alerts on iPhone and CarPlay. Independent development with coding agents. Responsible for app architecture, AI integration, and verification. Swift code classifies alert status before the model receives supplied facts. The AI integration checks model availability, limits generation time, handles cancellation, validates output, and falls back deterministically when needed. Separately built a bounded Swift agent/tool runtime with a 38-case scripted evaluation corpus and documented real-device validation. Checks cover tool selection, execution budgets, malformed results, cancellation, deadlines, and fallback behavior. This runtime is separate from the released country-summary feature. Released on the App Store; separately evaluated a Swift agent/tool runtime.

**Technologies:** SwiftUI · Swift Concurrency · CarPlay · Core Location · MapKit · URLSession · Apple Foundation Models · Structured Outputs · Tool Calling · Cancellation · Evaluation Corpus · Swift Testing

[App Store](https://apps.apple.com/app/id6793023910)

[Source code](https://github.com/vil4max/regional-check)

### OneCart Family

OneCart Family is a family shopping app with a shared iCloud list and purchase history. Independent development with coding agents. Responsible for product, implementation, and release quality. Core Data uses private and shared CloudKit stores with CKShare invitations. Edits persist locally before cloud propagation. The app handles membership changes, duplicate records, and recovery when cloud account deletion fails. WidgetKit snapshots and App Intents support widget actions. XCTest regression suites cover cart state, sharing, persistence, synchronization errors, and deletion recovery. I reviewed generated changes, investigated defects, and verified releases. Released on the App Store.

**Technologies:** Swift · SwiftUI · Swift Concurrency · Core Data · CloudKit · CKShare · WidgetKit · App Intents · XCTest · Offline Persistence · Synchronization Recovery

[App Store](https://apps.apple.com/app/id6793219621)

[Source code](https://github.com/vil4max/OneCart)

## Interests

- Long-term software product development
- Fintech products
- Teams using AI in everyday engineering
- Opportunities to contribute beyond iOS over time
