# Chain-of-Thought Calculator — Budget • Schedule • Travel (No API Key)

A mini, auditable reasoning tool that solves real-life math/logic problems step-by-step.

**Why this matters (for recruiters):**
- **Structured reasoning:** Plan → Work → Answer
- **Verified outputs:** Auto-grader and self-check pass/fail
- **Real-world tasks:** Budgeting (KES), scheduling (HH:MM), travel layovers
- **Zero-friction demo:** Works without an API key in Google Colab

---

## ✨ What it does
- Parses numbers/times from natural language
- Produces a clean, auditable solution:
  - **Plan** (≤3 short bullets)
  - **Work** (clear calculation lines)
  - **Answer** (single, bold final result with units)
- Double-solves and compares results (✅ MATCH / ⚠️ MISMATCH)

---

## 📚 Notebook
- **Colab:** `Chain_of_Thought_Calculator.ipynb`  
  - Open in Colab → Run top-to-bottom → Try **Interactive Solver** cell

> Optional: If you later add an API key, the same notebook can call a live LLM, but it’s not required.

---

## 🧪 Tests Included
- **Budgeting:** “I have 1,200 KES… spend 300 + 250… How much remains?” → **650 KES**
- **Scheduling:** “Start 09:20, lasts 45m, need 15m walk… When leave?” → **10:05**
- **Travel:** “Arrive 10:40, depart 12:05… Layover?” → **85 minutes**

The suite prints **Plan/Work/Answer** and **PASS** checks.

---

## 🚀 How to Run (Colab, free)
1. Upload the notebook to Google Colab (File → Upload Notebook)  
2. Run the cells in order:
   - Step 2: Template & caller (fallback demo if no key)
   - Step 3: Tests + auto-checker
   - Step 4: Self-check (double-solve)
   - Step 5: **Interactive Solver** (type your own problem)
3. That’s it. No API key needed.

---

## 🧠 Design Choices
- **Policy-friendly chain-of-thought:** We show a short, auditable plan and calculation lines (not long inner monologues).
- **Deterministic demo solver:** Ensures the notebook runs without external services.
- **Evaluator & self-check:** Treat AI math like production code—verify.

---

## 🧩 File Tree
├── Chain_of_Thought_Calculator.ipynb
├── README.md
└── /assets
├── screenshot_budget_pass.png
├── screenshot_schedule_pass.png
└── screenshot_interactive.png


---

## 📸 Suggested Screenshots
- Test suite output with **PASS** badges
- A Budgeting example (Plan/Work/Answer visible)
- Interactive run (your free-text input → result + ✅ MATCH)

---

## 🔒 Security & Safety
- No secrets in repo. Optional API key is entered at runtime only.
- Clear error messages if input is missing data (asks one clarifying question).

---

## 🏷️ Keywords
`prompt engineering` · `chain-of-thought` · `reasoning` · `structured outputs` · `validation` · `python` · `colab` · `regex parsing` · `testing` · `self-check`

---

## 📜 License
MIT


