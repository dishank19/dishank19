<!-- Profile README -->

<h1 align="center">Dishank Jhaveri</h1>
<p align="center">
  <i>AI Engineer — voice agents, tool-calling LLMs, and RL-tuned decision systems</i><br/>
  <a href="mailto:dishankjhaveri@gmail.com">dishankjhaveri@gmail.com</a> ·
  <a href="https://linkedin.com/in/dishankjhaveri">LinkedIn</a> ·
  <a href="https://github.com/dishank19">GitHub @dishank19</a>
</p>

---

### What I build
-  **Voice AI agents** that actually do work: answer calls, extract facts, take action.
-  **Agentic systems** with reliable tool access (LangGraph + MCP) and guardrails.
-  **Production infra** on GCP/AWS with clean observability and sane autoscaling.

> Ship real agents for real teams—safely, fast, and at scale.

---

## Featured work (from my pins)

**PatientIntakeVoiceAgent**  
`Python · FastAPI · Pipecat · OpenAI · Cartesia TTS · Twilio · Docker`  
Production-style voice intake: turn-taking, info capture, slot-filling, warm handoff.  
`dishank19/PatientIntakeVoiceAgent`

**Google_Ads_Agent**  
`Python · FastAPI · GAQL · LLM tool-use`  
Agent that researches keywords, adjusts bidding strategies, and manages ad groups.

**leadgen-agent**  
`Python · Retell/Voice · Twilio · SendGrid`  
Dental lead qualification: clinic lookup, appointment simulation, notifications + transcripts.

**Mistral7B_Finetune**  
`PyTorch · QLoRA · PEFT · HF Transformers`  
Fine-tuned Mistral-7B on SHP for AskHistorians-style long-form responses.

---

## Currently building & learning

- **PrimeIntellect** — a compact, RL-first **agent runtime**:
  - modular planner + memory, **policy interface** (PPO/SAC/BC) that can drive LangGraph edges,
  - environment adapters (dialog, keyword bidding, handoff) with KPI-based rewards,
  - **safety layer** (critics, budgets, escalation) and a clean eval → canary → prod path.

- **verifiers** — a lightweight **verification library** for agents:
  - composable checks for schema + invariants + semantic tests (e.g., “did we collect name + phone?”, “is PII redacted?”, “latency under 800ms?”),
  - returns **Score / Decision / Trace** objects; drop-in on LangGraph edges and tool results,
  - doubles as an offline eval harness for shadow runs and gates before promotion.

- **RL-tuned policies & custom envs** — train policies inside simulated funnels (dialog / GAQL keyword / handoff) to optimize **business KPIs** instead of proxy metrics. Rewards blend goal attainment, latency budgets, and safety constraints.

