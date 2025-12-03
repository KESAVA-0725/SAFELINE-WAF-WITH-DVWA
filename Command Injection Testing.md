# ⭐ 2. Command Injection Testing

# 🔸 What is Command Injection?

This vulnerability allows an attacker to inject system commands into an input field, letting them execute Linux commands on the server.

# 🔸 What you tested:

Performed DVWA command injection tasks using payloads like:

    127.0.0.1; ls
    8.8.8.8; cat /etc/passwd 


![image](https://github.com/KESAVA-0725/SAFELINE-WAF-WITH-DVWA/blob/main/images/Screenshot%202025-12-04%20024059.png?raw=true)

Attempted to bypass filters using encoded payloads.

# 🔸 SafeLine Operation Modes (very important):

SafeLine provides protection modes such as:

    Mode	       Behavior
    Disabled	WAF does not block anything
    Audit	    Logs the attack but allows the traffic
    Balanced    Blocks common attacks, allows normal traffic
    Strict	    Highly aggressive blocking, preferred for high-security environments
    
# 🔸 Observed Results:

Strict mode blocked all malicious commands immediately.

Audit mode logged the attack but still executed the request.

Balanced mode allowed safe inputs and blocked obvious attack patterns.
