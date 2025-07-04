# AAD-auth-demo
Azure Active Directory / Entra ID

This project demonstrates how to test Azure Active Directory (AAD) authentication using a test user account and verify the returned ID token using `jwt.ms`.

---

## 🎯 Goal

To simulate an AAD login flow, capture the returned ID token via redirect URI, and decode the JWT token for inspection—**without building a full-stack or production application**.

---

## 🔐 What This Project Does

- Initiates login for a test AAD user (`testuser01`)
- Captures ID token via the `localhost:3000` redirect
- Manually extracts the token from the URL
- Decodes and validates token claims at [jwt.ms](https://jwt.ms)

---


### 1. Azure AD Sign-In Prompt
<img width="1440" alt="Screenshot 2025-07-03 at 1 29 23 PM" src="https://github.com/user-attachments/assets/e73ccb01-f61c-42f6-8add-392623d82644" />


### 2. Token Returned in Redirect URI
<img width="1440" alt="Screenshot 2025-07-03 at 1 40 35 PM" src="https://github.com/user-attachments/assets/7e0ba27e-a257-4534-a279-8b80971e5005" />


### 3. Decoded Token in jwt.ms
<img width="1440" alt="Screenshot 2025-07-03 at 5 17 57 PM" src="https://github.com/user-attachments/assets/0983d6d2-2da5-41d1-9753-c2ae93162df5" />



---

## 🧠 What You Learn from This

- Basics of Azure AD authentication flows
- How ID tokens are returned and structured
- How to decode and inspect JWT tokens
- How AAD enforces app permission and consent policies

---

## 📝 Note

This is not a full-stack app. There is **no backend server** or persistent data storage. It is purely a test of the login and token flow with AAD.
