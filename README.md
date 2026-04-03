🛡️ Phishing Email Detection & Analysis Project

📌 Project Title

Task 2 – Phishing Email Analysis using Kali Linux Tools



📖 Overview

This project focuses on identifying and analyzing phishing emails using both content-based analysis and technical investigation tools in Kali Linux. Phishing is one of the most common cybersecurity threats, where attackers attempt to trick users into revealing sensitive information such as passwords, financial data, or personal details.

The goal of this project is to:
 • Understand how phishing emails are structured
 • Identify common phishing indicators
 • Analyze suspicious domains using technical tools
 • Draw conclusions based on evidence

This project simulates a real-world cybersecurity investigation workflow.
📂 Project Structure
task2-phishing-analysis/
│
├── README.md
├── report/
│   └── phishing_report.pdf
│
├── samples/
│   ├── email1.txt
│   └── email2.txt
│
├── analysis/
│   ├── whois_results.txt
│   ├── nslookup_results.txt
│   └── curl_results.txt
│
└── screenshots/
    ├── whois.png
    ├── nslookup.png
    └── curl.png

📧 Email Samples Description

📄 Email 1 – Prize Scam

Subject: Congratulations! You Won a Prize 🎉

This email claims that the recipient has won a $5000 prize and urges immediate action to claim the reward.

Key Characteristics:
 • Creates excitement and urgency
 • Promises unrealistic rewards
 • Includes a suspicious link
 • Uses generic greeting (“Dear Customer”)

Phishing Link:
http://claim-your-reward-now.com
📄 Email 2 – Security Alert Scam

Subject: Security Alert: Suspicious Login Attempt

This email warns the user of a suspicious login attempt and pressures them to verify their identity.

Key Characteristics:
 • Creates fear and urgency
 • Threatens account suspension
 • Requests immediate verification
 • Uses generic greeting (“Dear User”)

Phishing Link:
http://account-security-check.com

🔍 Analysis Methodology

The analysis was conducted in two main phases:

1. Content Analysis

Each email was examined for common phishing indicators, including:
 • Urgent or threatening language
 • Emotional manipulation (fear, excitement)
 • Suspicious or fake links
 • Generic greetings
 • Lack of personalization



2. Technical Analysis

The following Kali Linux tools were used:

🧪 WHOIS
Used to retrieve domain registration details such as:
 • Domain owner
 • Registration date
 • Registrar information

🌐 NSLOOKUP
Used to check:
 • Domain existence
 • DNS resolution
 • Associated IP address

🔗 CURL
Used to:
 • Test website connectivity
 • Retrieve HTTP headers
 • Identify server response


🧾 Analysis Results

🔎 Whois Results

Both domains:
 • Returned “No match”
 • Indicate that the domains are not registered or inactive

👉 This is highly suspicious because legitimate organizations always have registered domains.



🌐 Nslookup Results

Both domains returned:
NXDOMAIN (Non-Existent Domain)

👉 This means:
 • The domains do not exist in the DNS system
 • No IP address is associated with them



🔗 Curl Results

Both domains failed with:
Could not resolve host
👉 This confirms:
 • No active web server exists
 • The links are not functional



🚨 Phishing Indicators Identified

The following indicators confirm phishing activity:
 • ❗ Urgent and threatening language
 • 🎁 Fake rewards and promises
 • 🔗 Suspicious and non-existent links
 • 👤 Generic greetings
 • ⚠️ Pressure to act immediately
 • 🌐 Domains with no registration or DNS records


⚠️ Risk Classification

Both email samples are classified as:

HIGH RISK – PHISHING ATTEMPTS



🔄 How the Attack Works
 1. The attacker sends a fake email pretending to be legitimate
 2. The email includes a malicious or fake link
 3. The user clicks the link
 4. The user is redirected to a fake website (if active)
 5. The attacker collects sensitive information

In this case, the domains are inactive, which suggests:
 • The phishing campaign may have been taken down
 • The domains were temporary or disposable



🛡️ Prevention Methods

To protect against phishing attacks:
 • Avoid clicking unknown or suspicious links
 • Always verify the sender’s email address
 • Check for HTTPS and valid domains
 • Be cautious of urgent or emotional messages
 • Use antivirus and spam filters
 • Enable multi-factor authentication (MFA)


✅ Do’s and ❌ Don’ts

✅ DO:
 • Verify email authenticity
 • Report suspicious emails
 • Use strong, unique passwords

❌ DON’T:
 • Click unknown links
 • Share personal information
 • Trust emails that create panic or excitement


🧠 Key Insights

This project highlights an important concept:

Even the absence of data (no domain, no DNS, no server) is strong evidence of phishing.

Attackers often use:
 • Temporary domains
 • Disposable infrastructure
 • Short-lived campaigns



📌 Conclusion

Phishing remains a major cybersecurity threat due to its simplicity and effectiveness. Through both content and technical analysis, this project demonstrates how phishing emails can be identified and investigated.

The analyzed emails showed clear signs of phishing, supported by:
 • Suspicious content
 • Non-existent domains
 • Failed technical lookups

Awareness, verification, and critical thinking are essential defenses against such attacks.



🚀 Future Improvements
 • Analyze active phishing domains
 • Use additional tools (e.g., Wireshark, VirusTotal)
 • Automate phishing detection
 • Expand dataset with more email samples

⸻

👨‍💻 Author

TEMEN ALEMAYEHU
Cybersecurity Student Project – Kali Linux Phishing Analysis
