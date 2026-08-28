# RecoverAI
AI-powered revenue recovery agent for merchants using Razorpay Test Mode.

## Problem

Merchants lose revenue when payments fail, customers abandon checkout,
subscriptions fail, or receivables become overdue.

RecoverAI detects revenue at risk, diagnoses the reason, decides the
appropriate recovery action, executes bounded recovery workflows, verifies
payment status, and measures recovered revenue.

## Tech Stack

1. Razorpay Test Mode — payment and order infrastructure
2. n8n — workflow orchestration and automation
3. Python — backend logic and evaluation
4. FastAPI — backend API layer
5. Gemini API — AI diagnosis fallback and recovery decisions
6. SQLite — data storage
7. Streamlit — merchant dashboard
8. Docker — local development environment
9. GitHub — version control and documentation
10. Postman — API testing

## Core Recovery Actions

- Retry
- Reminder
- Human Review
- Do Nothing

## Core Principles

- No confirmed payment = no fulfillment
- AI recommendations are subject to deterministic policy rules
- High-risk actions require human review
- Recovery attempts have stopping rules
- Every money-related decision is auditable
- Performance is measured on 100+ synthetic cases
- Payment status is never assumed from an AI decision
