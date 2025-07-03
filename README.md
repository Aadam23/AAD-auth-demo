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
<img width="1440" alt="Screenshot 2025-07-03 at 1 29 23 PM" src="https://github.com/user-attachments/assets/e73ccb01-f61c-42f6-8add-392623d82644" />


### 2. Token Returned in Redirect URI
<img width="1440" alt="Screenshot 2025-07-03 at 1 40 35 PM" src="https://github.com/user-attachments/assets/7e0ba27e-a257-4534-a279-8b80971e5005" />


### 3. Decoded Token in jwt.ms
<img width="1440" alt="Screenshot 2025-07-03 at 5 17 57 PM" src="https://github.com/user-attachments/assets/0983d6d2-2da5-41d1-9753-c2ae93162df5" />



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
