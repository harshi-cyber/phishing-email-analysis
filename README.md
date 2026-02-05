# Phishing Email Analysis (SOC Lab)

This project demonstrates real-world phishing email analysis using standard SOC investigation techniques.
Multiple emails were analyzed to determine whether they were legitimate or malicious.

## Objective
To analyze suspicious emails and classify them as legitimate or phishing using technical and contextual indicators.

## Methodology
- Email header analysis
- SPF, DKIM, and DMARC validation
- Domain age and reputation checks
- URL and attachment analysis
- Content and social engineering review

## Tools Used
- MXToolbox
- VirusTotal
- WHOIS Lookup

## Email Analysis Summary

### Case 1: Prime Minister’s Office Email
- Classification: Legitimate  
- Risk Level: Low  
- Authentication: SPF, DKIM, DMARC passed  
- Verdict: Safe email, no action required
  ![image]

### Case 2: Let’s Defend Discount Email
- Classification: Legitimate (Marketing)  
- Risk Level: Low  
- Notes: Return-path difference due to Mailchimp  
- Verdict: Safe promotional email
![image]

### Case 3: WordUp Black Friday Email
- Classification: Legitimate (Bulk Marketing)  
- Risk Level: Low  
- Notes: DMARC failed due to third-party alignment  
- Verdict: Non-malicious
![image]

### Case 4: MyBharat Scholarship Email
- Classification: Legitimate  
- Risk Level: Low  
- Notes: Government domain verified  
- Verdict: Safe email
![image]

### Case 5: WebBoost Internship Email
- Classification: Phishing / Scam  
- Risk Level: High  
- Indicators:
  - Newly registered domain
  - BCC usage
  - Redirection to WhatsApp
  - No verified organization presence
- Verdict: Confirmed phishing attempt
  ![image]

## Key Learnings
- Passing SPF/DKIM/DMARC does not guarantee legitimacy
- Domain age and context are critical indicators
- Social engineering is a major phishing technique
- SOC analysts must correlate multiple signals

## Conclusion
Five real-world emails were analyzed. Four were legitimate, and one was confirmed as phishing.
This project reflects practical SOC email investigation and decision-making skills.
