# NotchPilot — User Privacy Choices & Data Rights

**Your Privacy Rights and Controls in NotchPilot**

Under privacy regulations worldwide—including the European Union General Data Protection Regulation (GDPR), California Consumer Privacy Act (CCPA), and Apple App Store Privacy Guidelines—users have the right to inspect, control, and opt out of data collection and behavioral profiling.

---

## 🛡️ Summary of Privacy Controls

Because NotchPilot operates with **Zero Data Collection**:

1. **No Tracking Opt-Out Necessary**:  
   NotchPilot does not track users across apps or websites. Apple's App Tracking Transparency (ATT) framework is not required because tracking is fundamentally non-existent in our codebase (`NSPrivacyTracking = false`).

2. **No Data to Delete or Access (DSAR / Right to Be Forgotten)**:  
   Since we never collect, store, or process any personal data, email addresses, or usage logs on our servers, there is zero stored data to export, modify, or delete.

3. **Local Reset**:  
   All user preferences (such as selected color theme, hover delay, or preferred display mode) are stored strictly on your Mac in local `UserDefaults`. To delete all local settings, simply remove the app or run:
   ```bash
   defaults delete com.notchpilot.app
   ```

4. **In-App Purchase Records**:  
   Your license status is tied securely to your Apple ID through Apple StoreKit 2. To manage or review purchase history, visit your [Apple ID Account Settings](https://appleid.apple.com) or the macOS App Store account page.

5. **Inquiries**:  
   If you wish to make a formal privacy rights request or have questions, contact: `support@notchpilot.app`.
