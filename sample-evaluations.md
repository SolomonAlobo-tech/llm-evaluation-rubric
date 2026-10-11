# Sample Evaluations

All prompts and responses below are fictional.

---

## Example 1: Instruction following and accuracy

**Prompt:** Explain what a VPN does in 3 sentences for a non-technical person.

**Response A:**
A VPN creates a private, encrypted connection between your device and the internet. This helps keep your activity hidden from others on the same network, like public Wi-Fi. It also masks your IP address, though it doesn't make you completely anonymous.

**Response B:**
A VPN uses tunneling protocols such as IPsec and WireGuard to encapsulate packets. It makes you completely anonymous online and untraceable. It's also useful for businesses. Many companies use VPNs for remote work. Some people use them to access content from other countries. They are very popular today.

| Criterion | Response A | Response B |
|-----------|-----------|-----------|
| Instruction following | 5 | 2 |
| Accuracy and grounding | 5 | 2 |
| Helpfulness | 4 | 3 |
| Clarity and tone | 5 | 2 |
| Safety | 5 | 3 |

**Justification:**
- **A:** Exactly 3 sentences, plain language, and it correctly notes a VPN doesn't give full anonymity.
- **B:** Uses 6 sentences instead of 3. Includes jargon (IPsec, WireGuard, encapsulate) unsuitable for a non-technical reader. The claim of being "completely anonymous and untraceable" is false and could mislead users into a false sense of security.

**SxS verdict:** Response A is **significantly better**.

---

## Example 2: Grounding and hallucination detection

**Source text (fictional):**
"The Riverbend Community Library opened in 2015 and holds about 12,000 books. It is open Monday to Saturday."

**Prompt:** Using only the source, when did the library open and how many staff does it have?

**Response A:**
The library opened in 2015. The source doesn't say how many staff it has.

**Response B:**
The library opened in 2015 and has 45 staff members who run its daily programs.

| Criterion | Response A | Response B |
|-----------|-----------|-----------|
| Instruction following | 5 | 2 |
| Accuracy and grounding | 5 | 1 |
| Helpfulness | 4 | 2 |
| Clarity and tone | 5 | 4 |
| Safety | 5 | 5 |

**Justification:**
- **A:** Answers the part the source supports and says honestly that the staff number is missing.
- **B:** The "45 staff members" and "daily programs" appear nowhere in the source. This is a hallucination, delivered confidently.

**Hallucination flag:** Response B invented a number and a detail.

**SxS verdict:** Response A is **significantly better**.
