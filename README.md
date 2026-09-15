# Max Vilchevskiy

**Senior iOS Engineer | AI-Enabled Software Development**

Kyiv, Ukraine · Remote

[vil4max@gmail.com](mailto:vil4max@gmail.com) · [Telegram](https://t.me/vil4max) · [LinkedIn](https://www.linkedin.com/in/vil4max/) · [Portfolio](https://vil4max.github.io) · [GitHub](https://github.com/vil4max)

[Resume PDF](https://vil4max.github.io/assets/Max_Vilchevskiy_Senior_iOS_Engineer.pdf) · [Portfolio](https://vil4max.github.io/)

## About

I'm a Senior iOS Engineer with 13 years of experience in iOS, consumer products, and fintech. I've built apps from scratch and worked on established products through years of growth. At Drinkit, I was part of the team that launched the app with its first coffee shop. At Umico, I developed marketplace features as the product grew into Birmarket, then built a subscription SDK for several host apps. My recent work also includes a watchOS voice client with an iPhone relay.

I'm looking for Senior iOS Engineer roles on long-term products, particularly in iOS and fintech. I can take a feature from technical planning through implementation and release, and I'd like to contribute to other parts of the product over time. AI-enabled development is part of how I work day to day.

## Focus

Swift · UIKit · SwiftUI · Swift Concurrency · Modular Architecture · Swift Package Manager (SPM) · URLSession · XCTest · Xcode Instruments · AI-Assisted Development · Coding Agents · Agentic Workflows · Context Engineering · Apple Foundation Models

## Apps

### DriveCheckUA

DriveCheckUA displays regional safety alerts on iPhone and CarPlay. Built independently with coding agents. Architected the client, on-device AI integration, and CarPlay UI. Swift code classifies alert status before the model receives supplied facts. The AI integration checks model availability, limits generation time, handles cancellation, validates output, and falls back deterministically when needed. Separately built a bounded Swift agent/tool runtime with a 38-case scripted evaluation corpus and documented real-device validation. Checks cover tool selection, execution budgets, malformed results, cancellation, deadlines, and fallback behavior. This runtime is separate from the released country-summary feature. Released on the App Store; evaluated a bounded Swift agent runtime.

**Technologies:** SwiftUI · Swift Concurrency · CarPlay · Core Location · MapKit · URLSession · Apple Foundation Models · Structured Outputs · Tool Calling · Cancellation · Evaluation Corpus · Swift Testing

[App Store](https://apps.apple.com/app/id6793023910)

[Source code](https://github.com/vil4max/regional-check)

### OneCart Family

OneCart Family is a family shopping app with shared iCloud lists. Built independently with coding agents. Led architecture, data synchronization, and release verification. Core Data uses private and shared CloudKit stores with CKShare invitations. Edits persist locally before cloud propagation. The app handles membership changes, duplicate records, and recovery when cloud account deletion fails. WidgetKit snapshots and App Intents support widget actions. XCTest regression suites cover cart state, sharing, persistence, synchronization errors, and deletion recovery. I reviewed generated changes, investigated defects, and verified releases. Released on the App Store.

**Technologies:** Swift · SwiftUI · Swift Concurrency · Core Data · CloudKit · CKShare · WidgetKit · App Intents · XCTest · Offline Persistence · Synchronization Recovery

[App Store](https://apps.apple.com/app/id6793219621)

[Source code](https://github.com/vil4max/OneCart)
