# NotchPilot — App Store Server Notifications Architecture

**Document Version: 1.0 (StoreKit 2 On-Device Architecture)**

---

## Architecture Overview

NotchPilot implements **Apple StoreKit 2** using on-device cryptographic receipt and JWS (JSON Web Signature) transaction verification (`Transaction.currentEntitlements` and `Transaction.updates`).

Because NotchPilot operates with a **100% offline, privacy-first, zero-knowledge architecture**, it does not require an external application server to unlock purchases, enforce licenses, or gate user access. All entitlement evaluations take place cryptographically on the user's Mac.

---

## App Store Server Notifications V2 Configuration

If you configure external server notifications in App Store Connect for automated webhook logging or analytics dashboards:

* **Notification Specification**: App Store Server Notifications V2 (JSON Web Signature)
* **Production Webhook URL**: `https://api.notchpilot.app/v2/appstore-notifications` (or placeholder for local offline entitlement architecture: `https://raresmihailcristea-cmyk.github.io/notchpilot/notifications/production`)
* **Sandbox Webhook URL**: `https://sandbox.api.notchpilot.app/v2/appstore-notifications` (or placeholder: `https://raresmihailcristea-cmyk.github.io/notchpilot/notifications/sandbox`)

> **Note for App Review**:  
> NotchPilot uses a client-side StoreKit 2 entitlement model (`StoreKitManager.swift`). No backend server is required for end users to purchase, restore, or enjoy the application.
