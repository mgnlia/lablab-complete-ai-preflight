# ShipFast Duo — Concept Brief

## One-Liner
Two collaborating AI agents that take a product idea from napkin sketch to validated, pitch-ready prototype in hours — built entirely inside Complete.dev.

## Problem Statement
Solo founders and small teams waste 2-4 weeks validating product ideas. They bounce between:
- Market research tools (TAM/SAM/SOM)
- Spec writing (Notion, Google Docs)
- Design tools (Figma)
- Prototyping (code editors)
- Pitch deck tools (Canva, Slides)
- Landing page builders

Each tool switch loses context. Each handoff introduces drift. The result: weeks of scattered work before knowing if the idea is even worth pursuing.

## Solution
**ShipFast Duo** is a 2-agent system inside Complete.dev that collapses the idea-to-pitch pipeline into a single collaborative workspace session:

### Agent 1: Strategist
**Role**: Product strategy, market validation, positioning

**Input**: Raw product idea (even just a sentence)

**Outputs**:
- Competitive landscape analysis
- Target market definition + sizing estimate
- User persona(s)
- Core value proposition
- Product spec with prioritized user stories
- Go-to-market strategy outline
- Structured brief for Builder agent

**System Prompt Core**:
```
You are Strategist, a product strategy expert. When given a product idea, you:
1. Analyze the competitive landscape
2. Define the target market and estimate size
3. Create 1-2 user personas
4. Craft a clear value proposition
5. Write a product spec with prioritized user stories
6. Outline a go-to-market strategy
7. Package everything into a structured brief for the Builder agent

Be concise, data-informed, and actionable. Focus on validation signals.
```

### Agent 2: Builder
**Role**: Technical implementation, design, marketing assets

**Input**: Structured brief from Strategist

**Outputs**:
- Component architecture
- Working prototype (frontend)
- Landing page copy + layout
- README with setup instructions
- Pitch deck (5-7 slides)

**System Prompt Core**:
```
You are Builder, a full-stack developer and designer. When given a product brief from Strategist, you:
1. Design a component architecture
2. Build a working frontend prototype
3. Create landing page copy and layout
4. Write a clear README
5. Generate a 5-7 slide pitch deck

Focus on speed and clarity. Ship something real, not perfect.
```

### Collaboration Flow
```
User → "I want to build [idea]"
  ↓
Strategist Agent
  → Market analysis
  → Product spec
  → GTM strategy
  → Structured brief
  ↓
Builder Agent
  → Architecture
  → Prototype
  → Landing page
  → Pitch deck
  ↓
User → Reviews, iterates, ships
```

## Meta-Recursive Demo Angle
The killer demo move: **use ShipFast Duo to validate and pitch ShipFast Duo itself.**

1. Feed "ShipFast Duo" as the product idea to Strategist
2. Strategist generates market analysis, spec, GTM for ShipFast Duo
3. Builder creates prototype and pitch deck for ShipFast Duo
4. Present the agent-generated pitch deck as the hackathon submission

This is genuinely impressive because:
- It proves the product works (self-referential validation)
- The demo IS the product
- Judges see the full pipeline in action
- It's memorable and original

## Technical Simplicity
- **No external infrastructure** — runs entirely in Complete.dev
- **No custom backend** — agents use Complete.dev's built-in capabilities
- **No deployment needed** — workspace IS the product
- **Leverages pre-built agents** — Architect, Strategy Agent, Copywriter as foundations
- **2 agents only** — minimum requirement, maximum simplicity

## Time Budget: 16 Hours Max

| Phase | Hours | Deliverable |
|-------|-------|-------------|
| Platform exploration | 2 | Familiarity with Complete.dev |
| Strategist agent design + testing | 4 | Working Strategist agent |
| Builder agent design + testing | 4 | Working Builder agent |
| End-to-end integration + meta-demo | 3 | Full pipeline working |
| Demo video + submission | 3 | Submitted project |
| **Total** | **16** | **Complete submission** |
