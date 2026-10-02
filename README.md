# Max Vilchevskiy

**Senior iOS Engineer | Agentic Engineering & Agent-Ready Apps**

Kyiv, Ukraine · Open to remote

Available immediately · Employment or contractor (FOP)

[vil4max@gmail.com](mailto:vil4max@gmail.com) · [LinkedIn](https://www.linkedin.com/in/vil4max/) · [GitHub](https://github.com/vil4max) · [Portfolio](https://vil4max.github.io) · [Telegram](https://t.me/vil4max)

[Resume PDF](https://vil4max.github.io/assets/Max_Vilchevskiy_Senior_iOS_Engineer.pdf) · [Portfolio](https://vil4max.github.io/)

## About

Senior iOS Engineer with 13 years of experience in iOS, consumer products, and fintech. Built apps from scratch and worked on established products through years of growth. Part of the team that launched the Drinkit app with its first coffee shop. At Umico, developed marketplace features as the product grew into Birmarket, then built a subscription SDK for three host apps. Recent work also includes a watchOS voice client with an iPhone relay.

Looking for two kinds of roles: Senior iOS Engineer positions on long-term products, particularly in consumer apps and fintech, and AI-native / agentic engineering roles centered on agent harnesses, context, tool calling, evaluation, and verification. Stampwork and my Swift agent/tool runtime are built on the same discipline. Able to take a feature from technical planning through implementation and release, and interested in contributing to other parts of the product over time.

## Focus

Swift · SwiftUI · UIKit · Swift Concurrency · Combine · Modular Architecture · Swift Package Manager (SPM) · Clean Architecture · XCTest · Xcode Instruments · AI-Assisted Development · Agentic SDLC · Coding Agents · Apple Foundation Models

### Stampwork

Stampwork is a kit for spec-driven iOS feature delivery with coding agents. Built by one engineer directing coding agents; a person approves the requirements and each iteration's plan, authorizes commits, and accepts each feature. The same engineer designs the process and builds its toolkit: task briefs, the runtime, the automated gate, and the independent review. A writer agent implements each task in its own worktree, the verify gate (format, lint, build, tests) runs locally and in hosted CI, and an independent review checks what the change introduced. The runtime each app installs is readable in its Tooling directory; the method, the tracing and brief tools, and the Claude Code plugin are private. Three public apps ship through it and are the evidence: DriveCheckUA and OneCart Family on the App Store, and PitStop on TestFlight.

**Technologies:** Agentic SDLC · AI-Assisted Development · Coding Agents · Claude Code · Codex · Model Context Protocol (MCP) · Deterministic Verification

## Apps

### DriveCheckUA

DriveCheckUA displays regional safety alerts on iPhone and CarPlay. Built independently with coding agents. Architected the client, on-device AI integration, and CarPlay UI. Swift code classifies alert status before the model receives supplied facts. The AI integration checks model availability, limits generation time, handles cancellation, validates output, and falls back deterministically when needed. Separately built a bounded Swift agent/tool runtime with a 38-case scripted evaluation corpus and documented real-device validation. Checks covered tool selection, execution budgets, malformed results, injection-like inputs, cancellation, deadlines, and fallback behavior. This runtime was separate from the released country-summary feature and has since been removed from the app. Released on the App Store; evaluated a bounded Swift agent runtime.

**Technologies:** SwiftUI · Swift Concurrency · CarPlay · Core Location · MapKit · URLSession · Apple Foundation Models · Structured Outputs · Tool Calling · Guardrails · Prompt Injection Testing · Cancellation · Evaluation Corpus · Swift Testing · StoreKit 2 · In-App Subscriptions · AI-Assisted Development · Agentic SDLC · Model Context Protocol (MCP) · Dependency Injection · Claude Code · Codex · Coding Agents · Context Engineering · Deterministic Verification · Human-in-the-Loop Engineering · WidgetKit · Live Activities · App Intents · Actors · Sendable · Swift 6

[App Store](https://apps.apple.com/app/id6793023910)

[Source code](https://github.com/vil4max/regional-check)

### OneCart Family

OneCart Family is a family shopping app with shared iCloud lists. Built with coding agents; a second developer contributed the Live Activity and Siri features. Led architecture, data synchronization, and release verification. Core Data uses private and shared CloudKit stores with CKShare invitations. Edits persist locally before cloud propagation. The app handles membership changes, duplicate records, and recovery when cloud account deletion fails. WidgetKit snapshots and App Intents support widget actions. XCTest regression suites cover cart state, sharing, persistence, synchronization errors, and deletion recovery. I reviewed generated changes, investigated defects, and verified releases. Released on the App Store.

**Technologies:** Swift · SwiftUI · Swift Concurrency · Core Data · CloudKit · CKShare · WidgetKit · App Intents · XCTest · Offline Persistence · Synchronization Recovery · AI-Assisted Development · Agentic SDLC · Dependency Injection · Claude Code · Codex · Coding Agents · Agentic Workflows · Deterministic Verification · UserNotifications · Actors · Sendable

[App Store](https://apps.apple.com/app/id6793219621)

[Source code](https://github.com/vil4max/onecart-ios)
