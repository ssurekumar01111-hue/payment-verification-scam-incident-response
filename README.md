# Fiverr Payment Verification Scam – Incident Response Case Study

## Overview
This repository documents a real-world social engineering and payment verification scam incident in which the author was the intended victim. The case study focuses on how the attack was delivered, how it was identified, and the defensive incident response actions taken to prevent financial loss.

The purpose of this project is to demonstrate practical cybersecurity awareness, incident response decision-making, and defensive security skills relevant to SOC Analyst and Blue Team roles.

---

## Incident Context

- **Role of Author:** Victim / Incident Responder
- **Platform:** Fiverr (Freelancing platform)
- **Incident Type:** Social Engineering / Financial Fraud Attempt
- **Attack Goal:** Theft of card details and forced advance payment
- **Outcome:** No financial loss; incident successfully contained

---

## Attack Description

The incident began when the author received a direct message on their Fiverr account from a user claiming that payment for a gig service had already been completed. The message instructed the author to confirm or receive the payment and included an external link.

After clicking the external link, the author was redirected to a fraudulent payment verification page impersonating a platform support or payment system. The page claimed that, as a first-time seller, identity and payment verification were required before funds could be released.

The fraudulent workflow requested sensitive financial information, including bank card details, and later demanded that the card maintain a minimum balance in order to complete a so-called “verification transaction.” The attacker attempted to legitimize the request by using professional language, references to security standards, and threats such as potential card blocking.

At no point did a legitimate order appear in the official Fiverr order dashboard, confirming that the payment claim was false. The interaction was identified as a payment verification scam relying on social engineering and platform impersonation.

---

## Indicators of Compromise (IOCs)

- Message claiming payment completion without an active order
- Redirection to an external website outside Fiverr
- Requests for card number, expiry date, and CVV
- Requests to disclose exact card balance
- Requirement to add funds to “unlock” payment
- Threats of card blocking if verification failed
- Generic support identity (e.g., named customer support agent)

---

## Detection & Analysis

The activity was classified as malicious based on the following observations:

- Fiverr does not require sellers to verify payments via external links
- Legitimate orders always appear in the platform’s order dashboard
- No platform requires sellers to pay or maintain balances to receive funds
- Requests for card details violate standard payment security practices
- The attacker relied on urgency, authority impersonation, and confusion

These characteristics align with known **social engineering–based payment verification scams**.

---

## Incident Response Actions Taken

1. Communication with the attacker was stopped immediately
2. The compromised bank card was permanently blocked
3. A replacement card with new credentials was requested
4. Multi-Factor Authentication (MFA) was enabled on all critical accounts
5. Passwords for email, platform, and banking services were changed
6. The attacker was reported and blocked on the freelancing platform
7. Browser data was cleared and device security checks were performed

---

## Impact Assessment

- **Financial Loss:** None
- **Card Exposure:** Yes (contained via immediate blocking)
- **Account Compromise:** No
- **Persistence Risk:** Mitigated
- **Incident Status:** Fully resolved

---

## MITRE ATT&CK Mapping

- **TA0001 – Initial Access**
  - Social Engineering (Impersonation)
- **TA0040 – Impact**
  - Attempted Financial Theft

---

## Lessons Learned

- Being the victim does not negate analytical or defensive responsibility
- Real attacks often target legitimate platforms to gain trust
- External payment requests are a critical red flag
- Rapid response significantly limits impact
- MFA and card controls are effective mitigation measures
- Defense-first awareness prevents escalation

---

## Preventive Recommendations

- Never click payment or verification links sent via messages
- Verify payments only through official platform dashboards
- Never provide card details, balances, or OTPs
- Enable MFA on all financial and work-related accounts
- Report suspicious activity immediately to platform support

---

## Skills Demonstrated

- Social engineering detection
- Fraud pattern recognition
- Incident response execution
- Risk assessment and containment
- Identity and access protection
- Security awareness and defensive mindset

---

## Author

**Surendra Kumar**  
Aspiring SOC Analyst | Defensive Cybersecurity  
GitHub: https://github.com/ssurekumar01111-hue
