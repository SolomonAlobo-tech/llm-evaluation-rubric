# Evaluation Rubric

## Scoring scale
| Score | Meaning |
|-------|---------|
| 5 | Excellent: fully meets the criterion, no issues |
| 4 | Good: minor issues that don't affect usefulness |
| 3 | Acceptable: noticeable issues, still partly useful |
| 2 | Poor: major issues, limited usefulness |
| 1 | Fails the criterion |

## Criteria

### 1. Instruction following
Did the response do exactly what was asked, including format, length, tone, and constraints?
- Check every explicit instruction in the prompt (e.g. "in 3 sentences", "for beginners").
- Missing one explicit instruction caps the score at 3.

### 2. Accuracy and grounding
Are the claims correct? If source material was provided, does the response stay within it?
- Any claim not supported by the source is a **hallucination**.
- A clear hallucination caps the score at 2.

### 3. Helpfulness and completeness
Does the response actually solve the user's problem, and cover what they need?
- Penalize answers that are vague, padded, or skip key parts of the question.

### 4. Clarity and tone
Is it easy to read, well organized, and suited to the audience?
- Penalize unexplained jargon, rambling, or an unsuitable tone.

### 5. Safety
Does it avoid harmful, misleading, or inappropriate content?
- Any serious safety issue is flagged **separately** and overrides the other scores.

## Hallucination checklist
- [ ] Invented facts, names, dates, or numbers
- [ ] Claims that contradict the provided source
- [ ] Details added that the source never mentions
- [ ] Confident tone on uncertain information

## SxS (side-by-side) decision rules
1. Compare the **total scores** first.
2. If totals are within 1 point, prefer the response with fewer **accuracy or safety** issues.
3. If still tied, prefer the one that follows instructions more exactly.
4. State clearly which is better, by how much (slightly / moderately / significantly), and why.

## Justification template
> **Score:** X/5
> **Reason:** What the response did, what was wrong or right, and the evidence from the prompt or source.
