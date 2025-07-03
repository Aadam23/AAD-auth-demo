# AAD-auth-demo
Azure Active Directory / Entra ID

This project verifies Azure AD authentication by simulating user login, capturing the redirect with an ID token, and manually decoding the token using jwt.ms. It serves as a frontend-only proof-of-concept to confirm that AAD login and token issuance work as expected.

---

## 🔐 Features
- Login with Azure AD test user (testuser01)
- Redirect URI token parsing
- Manual token validation and decoding
- JWT inspection via `jwt.ms`

---


### 1. Azure AD Sign-In Prompt
![Admin Approval](screenshots/azure-admin-approval.png)

### 2. Token Returned in Redirect URI
![Token in Localhost](screenshots/localhost-token-url.png)

### 3. Decoded Token in jwt.ms
![Decoded JWT](screenshots/jwtms-token-decoded.png)

---

## ⚙️ Tech Stack
- HTML / JavaScript (msal.js)
- Azure Active Directory
- jwt.ms for token decoding
- Safari for testing incognito auth flow

---

## 📝 Notes
- This project uses a test Azure tenant with restricted permissions.
- Admin consent is required for apps requesting directory-level scopes.
