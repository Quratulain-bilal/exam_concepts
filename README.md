# AI Agent Factory - Foundations Course Notes

Complete deep-dive notes for the **Foundations (Everyone)** track from [The AI Agent Factory](https://agentfactory.panaversity.org).

---

## 📚 Course Overview

| # | Course | Focus | Core Artifact |
|---|--------|-------|---------------|
| 1 | **Just Delegate It** | Mechanics of delegation | Delegation Brief (6 lines) |
| 2 | **AI Fluency (The 4Ds)** | Human competencies | 4D Mental Model |
| 3 | **Workflow Design & Diagnosis** | Team/system delegation | Delegation Map |
| 4 | **Governance, Risk & Responsible Use** | Safety/compliance gate | Governance Record (1 page) |

---

## 🎯 Course 1: Just Delegate It — Complete Deep Dive

### **Core Philosophy**
> Stop **asking** AI questions. Start **giving** AI jobs you can **verify**.

### **The Delegation Loop (6 Steps)**

```
DEFINE → DELEGATE → OBSERVE → INTERVENE → VERIFY → ACCEPT
```

| Step | Owner | Description |
|------|-------|-------------|
| **Define** | You | What result should exist |
| **Delegate** | You | Give AI responsibility |
| **Observe** | You watch, AI works | Let AI do routine work |
| **Intervene** | You | Correct/redirect when AI drifts |
| **Verify** | You | Check claims, numbers, sources |
| **Accept** | You | Decide: use it or send back |

**Rule:** *AI owns the middle. You own both ends.*

---

### **The Delegation Brief — 6 Lines (Core Artifact)**

```markdown
Outcome:     What exists when done? (e.g., "3 free courses compared, 1 recommended")
Context:     What AI can't know? (e.g., "Beginner, no coding, 5 hrs/week")
Constraints: Hard limits? (e.g., "Free only, no programming, current info")
Authority:   What may AI decide alone? (e.g., "Choose sources, pick shorter if equal")
Deliverable: What form? (e.g., "Table + 2-sentence rec, keep 'unverified' marks")
Verification: What will I check? (e.g., "Mark unconfirmed as 'unverified'")
```

> **This is a thinking tool, not a form.** Every disappointing result traces to one unanswered line.

---

### **11 Concepts Summary**

| Concept | Key Lesson | Exercise |
|---------|------------|----------|
| **1. Asking vs Giving Job** | Questions get answers; jobs get checkable results | Run opener job, check 1 link |
| **2. Outcome Not Clicks** | Describe result, not method | Rewrite job as outcome + 2 constraints |
| **3. Delegation Brief** | 6-line work order before AI starts | Write brief for running job |
| **4. Give AI Research** | Force search + source + date | Add "searched/knew + date" line |
| **5. Give AI Source** | "Use only this text, quote it, or say 'not in source'" | Paste course page, extract 3 facts |
| **6. Deliverable Not Answer** | Ask for file/table, preserve caveats | "Make downloadable doc, keep unverified" |
| **7. Authority** | Plan-first + decision boundaries | "List steps, wait for go" + boundaries |
| **8. The Job Again** | Projects = Knowledge + Standing Instructions | Create Project, add brief + source |
| **9. Intervene** | 4 moves: Correct, Redirect, Constrain, Clarify | Break job, fix with smallest message |
| **10. Verify** | Identify → Trace → Challenge → Decide | Check 1 claim end-to-end |
| **11. Portability Test** | Same brief → different AI = brief quality | Run brief in Claude + ChatGPT |

---

### **Delegation Record (Final Artifact)**

```
┌─────────────────────────────────────┐
│ BRIEF          │ 6 lines                      │
├─────────────────────────────────────┤
│ RUN            │ Model, date, Project used    │
├─────────────────────────────────────┤
│ CHECK          │ What verified, what found    │
├─────────────────────────────────────┤
│ DECISION       │ Accept / Correct / Investigate / Reject │
└─────────────────────────────────────┘
```

---

## 🧠 10 Zaheen-Level Questions & Deep Answers

### **Q1: Brief = Form ya Thinking Tool? Structure fixed kyun?**
**A:** Thinking tool. Structure = **cognitive offload**. 6 lines = minimum viable delegation (empirically derived). Kam = broken delegation, Zyada = bureaucracy.

### **Q2: Concept 2 (Outcome) vs Concept 7 (Plan-first) — Contradiction?**
**A:** Do layers:
- **Method** (Concept 2) = AI decides *how* at runtime
- **Plan approval** (Concept 7) = Human veto *before* start
Plan-first = cheapest Intervene moment.

### **Q3: Verification cost > delegation benefit?**
**A:** Isliye **Review Thresholds** (Stakes, Reversibility, Audience, Regulatory). Sirf threshold-crossing claims verify. Brief mein scope pehle define karo.

### **Q4: Perfect brief ke bawajood AI silent decisions/hallucinates?**
**A:** Brief **AI ko perfect nahi banata** — **tumhein visibility deta hai** ke kahan galat hua. Brief = contract. Breach visible hoti hai.

### **Q5: Portability test valid agar dono AI same hallucination karein?**
**A:** Test **hallucination catch nahi karta** — **tool-specific leakage catch karta hai**. Example: "Search current" → Claude searches, ChatGPT (no browse) uses memory. Test fail = brief tool-agnostic nahi.

### **Q6: 'Observe' vague hai — abdication to nahi?**
**A:** Observe = **Active monitoring**. Stream dekhna, pattern match Brief ke Deliverable se, early intervene trigger. Abdication = "baad mein dekh lunga."

### **Q7: Project mein 50 files → context window full?**
**A:** Project = retrieval mechanism, sab load nahi hota. **Real architecture:**
- Standing Instructions = System prompt (hamesha, chhota)
- Knowledge = RAG (relevant chunks only)
- Skills = Procedural knowledge (context-free)
**Zaheen move:** Sirf 3 cheezein Project mein: 1 Instruction, 1-2 Knowledge files, 1 Skill.

### **Q8: Redirect powerful hai, lekin destination tumhein pata hona chahiye?**
**A:** Redirect = **"Yahan mat jao, wahan jao"** — destination tum, path AI. Example: "Sirf official pricing page use karo" → AI dhundhta hai kaise navigate/extract karna.

### **Q9: Accountability meri, AI ki nahi → delegation ka incentive kahan?**
**A:** Incentive = **Speed + Scale**, not risk transfer.
| Without AI | With Delegation |
|------------|-----------------|
| 1 decision/day | 50 verifications/day |
| Scale = your bandwidth | Scale = AI bandwidth + your judgment |
**Risk transfer = Governance layer** (contracts, gates, audit) — next course.

### **Q10: Free account course = Paid workflow ka prototype?**
**A:** **Haan.** Pedagogical prototype = production skeleton.
| Free (Course) | Production |
|---------------|------------|
| Fresh chat | Project + Standing Instructions |
| Manual paste | Knowledge base / Connectors |
| Manual verify | Eval suites / Auto checks |
| You = gate | Designated reviewer + SLA |
| No Skills | Skills + Code exec + Tools |
**Course = Discipline. Tools = Implementation (har 6 mahine badalte hain).**

---

## 🔄 Course 2: AI Fluency (The 4Ds) — Preview

### **The 4Ds Framework**
```
Delegation  → Decide what AI should do
Description → Explain what you need (Product, Process, Performance)
Discernment → Judge results (confidence ≠ correctness)
Diligence   → Use responsibly, own outcome (Creation, Transparency, Deployment)
```

### **Three Modes of Working with AI**
| Mode | Human Role | AI Autonomy |
|------|------------|-------------|
| **Automation** | Script writer | Low (defined task) |
| **Augmentation** | Co-creator | Medium (thinking partner) |
| **Agency** | Director | High (pursues goal, you're not watching) |

---

## 🗺️ Course 3: Workflow Design & Diagnosis — Preview

### **Delegation Map (Step × Owner × Reason)**
| Step | Owner | Criterion | Carried By |
|------|-------|-----------|------------|
| Extract clauses | AI | Reversible, low stakes | Skill |
| Flag departures | AI | Reversible, checked next | Skill |
| Draft redline | Collaborative | High stakes | Skill + Gate |
| Compute exposure | AI | Reversible, checked at gate | Code execution |
| Approve changes | Human | **Accountability** | Named reviewer |
| Sign & send | Human | **Irreversible** | Named signer |

**Three Criteria per Step:**
1. **Reversibility** — Can it be undone?
2. **Stakes** — Cost of error in worst case?
3. **Accountability** — Who answers for outcome?

**Three Ownership Types:**
- **AI-appropriate** — AI owns it
- **Collaborative** — AI produces, human judges
- **Human-retained** — Human owns outright

### **Diagnosis: 4 Causes by Timing**
| When Symptom Appeared | Cause | Fix |
|----------------------|-------|-----|
| First response | Under-specification | Add missing context |
| Degraded over session | Context overload | New chat / compress |
| Repeatable error type | Wrong feature/model | Switch tool/tier |
| "Used to work" | Stale configuration | Update Project/Skill |

---

## ⚖️ Course 4: Governance, Risk & Responsible Use — Preview

### **Four Questions Before Meaningful Work**

| Question | Three Answers |
|----------|---------------|
| **1. The Case** — Can AI do this? | Fully appropriate / **With review** / Inappropriate |
| **2. The Data** — Can this info go in? | Green / **Yellow (check/control)** / Red |
| **3. The Capability** — Turn this on? | Enable / **Escalate** / Decline |
| **4. The People** — Unfair impact? | Decide & document / **Disclose** / Escalate |

**Middle answer = where professional judgment lives** (names reviewer, control, route, disclosure).

### **Data Tiers**
- **Green:** Public, aggregated, anonymized
- **Yellow:** Internal, PII, confidential — check route, redact
- **Red:** Secrets, regulated, privileged — approved route only

### **Capability Trust Check (5 Checks)**
1. **Source** — Who published?
2. **Reach** — What data/systems could it touch?
3. **Fit** — Proportionate to job?
4. **Outside Content** — Reads untrusted input?
5. **Actions** — Can send/pay/delete/approve?

---

## 📖 Learning Path

```
Week 1: Just Delegate It (hands-on, 3 hrs)
    ↓
Week 2: AI Fluency (mental model, 1 hr)
    ↓
Week 3: Workflow Design (team map, 2 hrs)
    ↓
Week 4: Governance (compliance gate, 1.5 hrs)
```

---

## 🎓 PCAO-F Exam Blueprint Mapping

| Domain | Concepts |
|--------|----------|
| D1: Prompting & Task Execution | 1, 3, 4, 7 |
| D2: Output Evaluation | 11 |
| D3: Product & Model Selection | 5, 6, 13 |
| D5: Config & Knowledge Mgmt | 9 |
| D6: Governance, Risk, Responsible Use | 8, 12 |
| D7: Troubleshooting | 10 |

---

## 🚀 Quick Start

```bash
# 1. Get free AI account (Claude/ChatGPT/Gemini)
# 2. Open course
open https://agentfactory.panaversity.org/docs/just-delegate-it-crash-course
# 3. Pick a "running job" (learn Python, Excel, public speaking...)
# 4. Do Concept 1 "Do It Now" → Concept 11
# 5. Build your Delegation Record
```

---

## 📎 Resources

- [Just Delegate It Course](https://agentfactory.panaversity.org/docs/just-delegate-it-crash-course)
- [AI Fluency Course](https://agentfactory.panaversity.org/docs/ai-fluency-crash-course)
- [Workflow Design Course](https://agentfactory.panaversity.org/docs/workflow-design-diagnosis-crash-course)
- [Governance Course](https://agentfactory.panaversity.org/docs/governance-risk-responsible-use-crash-course)
- [Certifications](https://agentfactory.panaversity.org/docs/certifications)
- [ChatGPT & Claude Quick Reference](https://agentfactory.panaversity.org/docs/claude-chatgpt-101-crash-course)

---

## 💡 Key Takeaway

> **Course tools nahi sikhata — discipline sikhata hai.**
> Tools har 6 mahine mein badlenge. Delegation Loop, Brief, Verification, Map, Governance Record — ye **permanent skills** hain.

---

*Notes compiled from The AI Agent Factory Foundations track. For certification: [PCAO-F Associate](https://agentfactory.panaversity.org/docs/certifications/pcao-f).*