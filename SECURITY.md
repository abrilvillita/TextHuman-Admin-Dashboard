# Security

This public repository contains an administrative browser client. It is not an authorization boundary. The Cloudflare Worker must authenticate and authorize **every** privileged request, independently of the UI, and should enforce rate limits and audit logging. A shared secret sent from a browser is a temporary design with significant exposure risk; replace it with individual administrator accounts, short-lived sessions and MFA before relying on this panel for production operations.

The client no longer persists the admin secret in localStorage. Older saved copies are removed when the updated page loads. Clear browser site data and rotate the server-side admin secret after deploying this change, especially on shared devices. Changing this file does not revoke previously exposed credentials or change the Worker.

Do not post real user records, payment details, credentials, or vulnerability details in public issues. Report security findings privately to the project owner through GitHub's private vulnerability reporting if enabled, or the contact route on the TextHuman site.
