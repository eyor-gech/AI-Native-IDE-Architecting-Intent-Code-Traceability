# AI-Native-IDE-Intent-Traceability

This repo contains enhancements for Roo-Code related to Intent → Code Trace Mapping.  
The base Roo-Code must be cloned separately:

```bash
git clone https://github.com/<your-username>/Roo-Code.git
cd Roo-Code
pnpm install
```

### 2️⃣ Folder Structure
Professional projects usually separate concerns. For your repo, a simple, clean structure could be:
```
/docs → architecture diagrams, design notes, flow explanations
/src → enhancement scripts / code for Intent → Code Trace
/demo → screenshots, sample logs, small examples
/README.md → instructions, setup, references to Roo code
/tests → unit tests or mini examples to validate your tracing.  
```

### 3️⃣ Trace Storage: JSON vs JSONL vs Others
Professionals often choose **JSONL (JSON Lines)** for append-only trace logs:  
- Each line = one Intent → Code mapping event  
- Easy to **append** without rewriting the entire file  
- Works well for **streaming, audits, and debugging**