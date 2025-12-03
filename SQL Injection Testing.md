# ⭐  SQL Injection Testing
🔸 What is SQL Injection?

SQL Injection allows an attacker to insert malicious SQL queries into an input field to access or manipulate the database.

![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-12-03%20222604.png?raw=true)

🔸 Examples tested:

    ' OR '1'='1

    ' UNION SELECT NULL, version()--

     admin' --


![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-12-03%20232515.png?raw=true)

🔸 SafeLine Behavior:

1. Automatically identified SQL-specific patterns.

![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-12-03%20232632.png?raw=true)

3. Highlighted malicious keywords (OR, UNION, SELECT)

4. Blocked unauthorized login attempts

5. Logged full attack details including:

*  Payload

* Source IP

* Matching security rule

![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-12-03%20232721.png?raw=true)
