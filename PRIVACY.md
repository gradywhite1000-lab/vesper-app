# Privacy Policy — Vesper

**Last updated: May 2026**

## Summary (plain English)

Vesper can connect to your bank accounts to automatically track transactions. When you use this feature, your financial data is stored securely in our cloud database (Supabase). Your **bank credentials are never seen or stored by Vesper** — that's handled entirely by Plaid, a regulated financial data platform used by thousands of apps. If you don't connect a bank, your data stays local on your device as always.

---

## Full Policy

### What data Vesper collects

Vesper operates in two modes:

**Manual mode (no bank connection):** All data you enter — income, expenses, net worth, savings goals — is stored exclusively on your device using local storage. This data is never transmitted anywhere.

**Bank-connected mode (optional):** When you connect a bank account via Plaid, the following data is stored in our secure cloud database (Supabase):
- Transaction history (merchant, amount, date, category)
- Account balances and account metadata (name, type, last 4 digits)
- A Plaid access token (encrypted) used to refresh your data
- Your Vesper user ID (linked to your account)

We do **not** store your bank username, password, PIN, or full account numbers — ever. Plaid handles authentication and we receive only the data described above.

### Bank Account Integration (Plaid)

Vesper uses [Plaid](https://plaid.com) to connect to your financial institutions. Plaid is a regulated financial data aggregator that:
- Handles your bank login credentials directly — Vesper never sees them
- Is subject to its own privacy policy and security standards
- Complies with applicable financial data regulations

When you connect a bank, you interact with Plaid's secure interface (Plaid Link). After authentication, Plaid provides Vesper with read-only access to your transaction and balance data.

Plaid's privacy policy: https://plaid.com/legal/#privacy-policy

You can disconnect your bank at any time from Vesper's settings. This revokes Plaid's access and deletes your stored bank data from our servers.

### Data Storage and Encryption

Bank-connected data is stored in Supabase, a secure cloud database platform:
- **In transit:** All data is encrypted using TLS (HTTPS)
- **At rest:** Data is encrypted using AES-256
- **Access control:** Your data is protected by row-level security — only your authenticated account can access it

Supabase's security overview: https://supabase.com/security

### AI Advisor

The AI advisor uses the Groq API to answer your questions. When you send a message, it is transmitted to Groq's servers along with a summary of your financial context (net worth, income, savings rate, recent spending). Groq's privacy policy applies. We do not store or log these conversations on our end.

Groq's privacy policy: https://groq.com/privacy

### Notifications

If you grant notification permissions, Vesper schedules local notifications on your device (streak reminders, budget alerts). These are processed entirely on-device and not transmitted anywhere.

### Face ID / Touch ID

Vesper uses your device's biometric authentication to protect the app. Your biometric data is never accessed or stored by Vesper — authentication is handled entirely by iOS's Secure Enclave.

### Crash Reporting & Analytics

None. Vesper does not include crash reporting or analytics SDKs.

### Data Retention

If you delete your account or disconnect all bank connections, your stored transaction and balance data is deleted from our servers within 30 days.

### Your Rights

You can:
- View all data Vesper holds about you
- Disconnect bank accounts and delete associated data at any time
- Request full account deletion by emailing us

### Changes to this policy

If anything material changes, we'll update the date above and describe what changed.

### Contact

Questions or data requests: gradywhite1000@gmail.com

---

**The short version:** Bank credentials = handled by Plaid, we never see them. Your transaction data = encrypted in Supabase. Manual data = still local-only. You're always in control.
