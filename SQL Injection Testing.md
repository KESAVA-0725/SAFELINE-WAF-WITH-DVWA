⭐ 3. SQL Injection Testing
🔸 What is SQL Injection?

SQL Injection allows an attacker to insert malicious SQL queries into an input field to access or manipulate the database.

🔸 Examples tested:

    ' OR '1'='1

    ' UNION SELECT NULL, version()--

     admin' --

🔸 SafeLine Behavior:

1. Automatically identified SQL-specific patterns.

2. Highlighted malicious keywords (OR, UNION, SELECT)

3. Blocked unauthorized login attempts

4. Logged full attack details including:

*  Payload

* Source IP

* Matching security rule
