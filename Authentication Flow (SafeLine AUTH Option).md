⭐ 4. Authentication Flow (SafeLine AUTH Option)

SafeLine provides an authentication mechanism that stands between users and the application.

# 🔸 What you implemented:

* Created authentication entries for test users.

* Configured username, password, and optional metadata.

# 🔸 User Login Process:

1. User enters credentials on the SafeLine-generated login page.

2. The login request is first sent to SafeLine.

3. SafeLine notifies the operator (you).

4. You can choose:

   * ALLOW → User is forwarded to DVWA

   * DENY → User is blocked

# 🔸 This demonstrates:

* Inline access control

* Real-time manual decision-making

* Session validation and user-level filtering
