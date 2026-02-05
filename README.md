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
  ![image]<img width="1280" height="939" alt="image" src="https://github.com/user-attachments/assets/005296a1-bb79-46d5-8262-c8c491be684e" />


### Case 2: Let’s Defend Discount Email
- Classification: Legitimate (Marketing)  
- Risk Level: Low  
- Notes: Return-path difference due to Mailchimp  
- Verdict: Safe promotional email
![image]<img width="1600" height="1233" alt="image" src="https://github.com/user-attachments/assets/4c50764d-b570-453e-96cf-24a27a4a62a6" />


### Case 3: WordUp Black Friday Email
- Classification: Legitimate (Bulk Marketing)  
- Risk Level: Low  
- Notes: DMARC failed due to third-party alignment  
- Verdict: Non-malicious
![image]<img width="1280" height="956" alt="image" src="https://github.com/user-attachments/assets/a4921db5-2ac9-4ec3-a208-9192e9c56791" />
  ![image]<img width="1280" height="786" alt="image" src="https://github.com/user-attachments/assets/b28086a0-e08d-4dd3-aaba-203a585d02a9" />
  ![image]<img width="1280" height="810" alt="image" src="https://github.com/user-attachments/assets/b8986111-ba6c-4d73-8102-c59896041cd7" />




### Case 4: MyBharat Scholarship Email
- Classification: Legitimate  
- Risk Level: Low  
- Notes: Government domain verified  
- Verdict: Safe email
![image]<img width="1280" height="936" alt="image" src="https://github.com/user-attachments/assets/797e5014-10cf-4f9a-9568-c7c65a863fcc" />
![image]<img width="1280" height="590" alt="image" src="https://github.com/user-attachments/assets/c7adb2db-39fb-4d7e-ac77-7a4ae70b667d" />


### Case 5: WebBoost Internship Email
- Classification: Phishing / Scam  
- Risk Level: High  
- Indicators:
  - Newly registered domain
  - BCC usage
  - Redirection to WhatsApp
  - No verified organization presence
- Verdict: Confirmed phishing attempt
  ![image]<img width="1280" height="1019" alt="image" src="https://github.com/user-attachments/assets/b620abbc-e160-4b96-a6e3-7ed3d9988a9b" />


## Key Learnings
- Passing SPF/DKIM/DMARC does not guarantee legitimacy
- Domain age and context are critical indicators
- Social engineering is a major phishing technique
- SOC analysts must correlate multiple signals

## Conclusion
Five real-world emails were analyzed. Four were legitimate, and one was confirmed as phishing.
This project reflects practical SOC email investigation and decision-making skills.
