# Privacy Policy for Flock Discord Bot

**Last Updated:** June 16, 2026

We respect your privacy and are committed to protecting any personal data processed by the **Flock** Discord Bot (the "Bot"). This Privacy Policy explains what data we collect, how it is used, how it is stored, and your rights regarding your information.

By adding Flock to your Discord server or interacting with it, you agree to the terms of this Privacy Policy.

---

## 1. Information We Collect

To provide security and moderation features, Flock processes and stores certain information from your Discord server interactions:

### A. Data Processed in Real-Time (In-Memory Only)
* **Message Content:** The text content and image attachments of standard chat messages are analyzed in-memory to scan for malicious links, phishing attempts, spam, and media previews. **Clean messages are never stored, logged, or saved to disk.**

### B. Data Stored Persistently (SQLite Database)
* **Discord User IDs & Usernames/Tags:** Used to track message counts, moderation history, and active verification sessions.
* **Guild (Server) and Channel IDs:** Used to maintain server-specific configurations (e.g. whitelisted channels, log channels).
* **Flagged Message Content:** If a message triggers the bot's anti-scam/phishing filters, the offending message text, matched URLs, and action details (timeout/soft-ban) are stored in the server's moderation log for audit review by server administrators.
* **Verification Attempts:** Tracks failed rules-verification quiz attempts and cooldown timestamps to prevent automated brute-forcing.

---

## 2. How We Use Your Information

We use the collected information solely for the following purposes:
* **Anti-Scam & Phishing Prevention:** Protecting your community by automatically deleting malicious links and images.
* **Dynamic Trust Management:** Adjusting moderation checks based on member server age and message volume to minimize false positives.
* **Server Verification:** Managing the rules-based onboarding flow for new members.
* **Moderation Logs:** Providing server administrators with audit records of the bot's automated enforcement decisions.

**We do NOT sell, rent, or share your data with any third-party services, nor do we use it to train AI or machine learning models.**

---

## 3. Data Retention & Deletion

We believe in minimal data retention:
* **Inactive Member Data:** The bot periodically runs a cleanup process that automatically deletes message counts and verification records for users who have left the server.
* **Moderation Audit Logs:** These are kept persistently at the discretion of server administrators. Server administrators can clear all logs and configurations at any time using the bot's administrative slash commands.
* **User Requests:** If you want your moderation history or verification counts deleted, you may contact the bot administrator directly (see Section 6).

---

## 4. Data Security

We take the security of your data seriously:
* Flock's database is stored locally on a secured host server.
* The host server utilizes industry-standard full disk encryption (FDE) at rest.
* Access to the database is restricted to the bot's system administrator.

---

## 5. Third-Party Services

Flock interacts with the following external service to verify malicious URLs:
* **URLhaus API:** We query domains to verify if they are flagged in the URLhaus database. No user-identifiable data (such as User IDs or message context) is sent to this API; only normalized URLs/domains are submitted for lookup.

---

## 6. Contact & Data Deletion Requests

If you wish to delete your personal data from Flock's database, you can do so automatically by joining our Support Server:

* **Support Server:** https://discord.gg/axa5nY2c5K
* **How to delete:** Join the server, navigate to the `#request-data-delete` channel, and click the **"Delete my data"** button. The process is fully automated.

For any other privacy-related questions or inquiries, you may contact the bot administrators in our Support Server.
