# Privacy Policy for NotchPilot

**Effective Date: October 12, 2026**

NotchPilot ("the Application", "we", "our") is developed by **Rareș-Mihail Cristea** as a native macOS utility built on a strict **Zero-Data-Collection Architecture**. Your privacy and the confidentiality of your computing environment are absolute.

---

## 1. Zero Personal Data Collection
NotchPilot **does not collect, harvest, store, transmit, or sell** any personal information, device identifiers (UDID/MAC), IP addresses, location data, or behavioral metrics. 

## 2. On-Device, Ephemeral Telemetry
All hardware utilization statistics displayed in the HUD—including CPU percentages, RAM footprint, storage volumes, network throughput, and battery diagnostics—are retrieved locally through native Apple kernel APIs:
* **Mach Kernel Interfaces** (`host_statistics64`, `processor_info`)
* **Darwin Socket Counters** (BSD `sysctl` network interface bytes)
* **Apple Metal & IOKit Frameworks** (GPU metadata and smart battery diagnostics)

All retrieved telemetry is processed **exclusively in volatile RAM** and updated at real-time polling intervals. Telemetry is **never written to persistent disk storage** and is **never transmitted across any local or wide-area network**.

## 3. No Network Communications & No Trackers
* **Zero Telemetry Endpoints**: NotchPilot does not make outbound network connections to analytics servers, telemetry collectors, or remote loggers.
* **No Third-Party SDKs**: The application contains no third-party tracking libraries, advertising SDKs, crash analytics trackers, or profiling pixels.
* **Network Meter Functionality**: The network speed counter merely measures raw packet byte deltas on your local hardware network interfaces. It never inspects packet contents, domain names, URLs, or network payloads.

## 4. In-App Purchases & Apple StoreKit 2
All financial transactions, license purchases, and receipt validations are handled natively and securely by **Apple StoreKit 2**. Payment information (credit cards, billing details, Apple ID credentials) is processed directly by Apple Inc. and is never accessed or stored by NotchPilot.

## 5. Apple Sandbox Compliance
NotchPilot complies with Apple's macOS App Sandbox security requirements, operating in an isolated, sandboxed container without unrestricted file system or device access.

## 6. Contact Information
For any inquiries or privacy-related questions:
* **Developer**: Rareș-Mihail Cristea
* **Email**: `rares.cristea@ymail.com`
* **Address**: Bucharest, Romania
