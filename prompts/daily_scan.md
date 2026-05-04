# Daily Mechanism-Driven Literature Scan Prompt

## Task

Generate a daily research paper scan focused on **mechanistic insights and high-value ideas**, not simple paper listing.

---

## Search Scope

Search papers from the past 24 hours from:

- PubMed  
- bioRxiv  
- medRxiv  
- Major journals (Nature, Science, Cell families)

---

## Focus

Prioritize:

1. Direct relevance to the target research topic  
2. Strong mechanistic insights  
3. Transferable ideas from other domains  

---

## Filtering Rules

Include:
- Mechanistic studies  
- Biologically meaningful findings  
- Cross-domain insights  

Exclude:
- Purely clinical reports  
- Imaging-only papers  
- AI-only work without biological insight  
- Low-mechanism descriptive studies  

---

## Ranking

Prioritize:

1. Relevance  
2. Mechanistic depth  
3. Novelty  
4. Transferability  

---

## Output Format

Organize into:

### 1. Direct relevance
### 2. Mechanistic insights

For each paper:

- English title  
- (Optional) title in your preferred language 
- Source  
- One-sentence novelty (EN)  
- One-sentence "Why useful" (EN)  
- DOI / link  

---

## Constraints

- Max 50 papers  
- Do NOT pad results  
- Keep concise (≤5 lines per paper)  

---

## Style

- No long summaries  
- High signal-to-noise  
- Easy to skim  

---
## Optional: Email Delivery

This prompt can be combined with an automated workflow to send reports via email.

- generate a daily report
- export as DOCX
- send to a configured email address

Implementation depends on your local setup or automation tools.

---
## Notes

- Avoid literal translation artifacts  
- Preserve technical terms (e.g. T cell, alpha-synuclein)  
- Clearly mark preprints  

---

## Output

Structured content suitable for DOCX or report generation.
