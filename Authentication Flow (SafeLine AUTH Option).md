⭐  Authentication Flow (SafeLine AUTH Option)

SafeLine provides an authentication mechanism that stands between users and the application.

# 🔸 What you implemented:

* Created authentication entries for test users.

![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-12-04%20010443.png?raw=true)

* Configured username, password, and optional metadata.

# 🔸 User Login Process:

1. User enters credentials on the SafeLine-generated login page.

![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-12-04%20010500.png?raw=true)

3. The login request is first sent to SafeLine.

![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-12-04%20010630.png?raw=true)

5. SafeLine notifies the operator (you).

6. You can choose:

   * ALLOW → User is forwarded to DVWA

   * DENY → User is blocked

![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-12-04%20010646.png?raw=true)

# 🔸 This demonstrates:

* Inline access control

* Real-time manual decision-making

* Session validation and user-level filtering
