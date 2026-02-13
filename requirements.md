# CouncilAI Dev

## 1. Overview

### Vision
CouncilAI Dev acts like a virtual senior engineering team that helps software teams understand codebases, debug production issues, and explain system behavior to different stakeholders.

---

## 2. Problem Statement

Modern engineering teams spend excessive time:
- Understanding large unfamiliar codebases
- Debugging using fragmented sources (logs, monitoring, code)
- Explaining technical behavior to non-technical stakeholders
- Validating AI outputs due to hallucination risks

Existing AI tools focus mainly on code generation rather than system reasoning and multi-perspective validation.

---

## 3. Target Users

### Primary Users
- Software Developers
- SRE / DevOps Engineers
- Engineering Managers / Tech Leads

### Secondary Users
- Product Managers
- Technical Investors / Stakeholders

---

## 4. Core Value Proposition

CouncilAI Dev enables teams to:

- Understand codebases visually using UML + architecture diagrams
- Debug production issues using logs + code correlation
- Improve answer reliability using multi-model AI reasoning
- Translate technical insights into stakeholder-friendly explanations
- Reduce onboarding and debugging time

---

## 5. MVP Scope

### 5.1 Codebase Intelligence Engine

#### Features
- Accept GitHub repository link
- Parse and analyze repository structure
- Generate UML diagrams:
  - Class Diagram
  - Sequence Diagram
  - Component Diagram
  - Package / Module Diagram
  - System Architecture Diagram
- Provide repository-based Q&A (RAG)

---

### 5.2 Codebase Q&A (RAG)

#### Capabilities
- Natural language question answering
- Context retrieval from repository
- Grounded answers using real code structure
- Persona-based explanation output

---

### 5.3 Debugging Copilot

#### Input Methods
- .txt log file upload
- Plain text log paste

#### Capabilities
- Log parsing (structured + unstructured)
- Anomaly detection
- Log-to-code correlation
- Root cause probability ranking
- Fix suggestions with reasoning

---

### 5.4 Mini Multi-LLM Council

#### Roles
- Chairman Model → Task orchestration
- Expert Models → Code + Debug reasoning
- Critic Model → Risk validation

---

### 5.5 Persona Translator

#### Personas
- Intern Mode
- CTO Mode
- Investor Mode
- Incident Mode
- Professor Mode

---

## 6. Functional Requirements

### Codebase Analysis
- System shall accept GitHub repository links
- System shall analyze repository structure
- System shall generate UML diagrams
- System shall generate architecture diagrams

### Repository Q&A
- System shall allow natural language questions
- System shall retrieve relevant code context
- System shall avoid hallucinating components

### Debug Analysis
- System shall accept logs via upload or paste
- System shall detect anomaly patterns
- System shall generate root cause ranking

### AI Council
- System shall route tasks via Chairman model
- System shall validate via Critic model
- System shall generate unified output

### Persona Translation
- System shall allow persona selection
- System shall convert explanation tone
- System shall support near real-time switching

---

## 7. Non-Functional Requirements

### Performance
- Analysis response < 60 seconds for medium repos
- Q&A response < 10 seconds

### Reliability
- Must provide confidence scores
- Must support multi-model validation

---

## 8. Constraints

- No automatic code modification
- Batch analysis only
- Prefer low-cost or local models
- Persona translation must be demo-ready

---