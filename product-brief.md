# tycostream Product Brief

This product brief is the foundation for tycostream positioning and messaging.

## Positioning

How to talk about tycostream

### Framework

The positioning framework has 6 parts:

1. **Functional description** — What is the product, who is it for, and what does it do
2. **Problem framing** — The core challenge the product solves
3. **Value framing** — The outcome and benefit the product delivers
4. **Supporting argument 1** — First proof point with features
5. **Supporting argument 2** — Second proof point with features
6. **Supporting argument 3** — Third proof point with features

### Anchors

Each part uses anchors to ground the message in something the audience already knows:

- **[category]** anchors what kind of product it is
- **[persona]** anchors who uses it
- **[use case]** anchors the business scenario or core job to be done
- **[problem]** anchors what's broken or painful about the status quo
- **[feature]** anchors what capabilities enable that
- **[value]** anchors the business outcome

---

### Functional Description

The functional description answers: what is the product, who is it for, and what does it do—without talking about use cases or outcomes yet.

> tycostream is a **GraphQL server** [category] that helps **backend developers** [persona] **build real-time APIs over their streaming database** [use case].

Each part of this sentence does specific work:
- **GraphQL server** is the category anchor—familiar, tells you what shelf it belongs on
- **Backend developers** is the persona anchor—the people responsible for making data available
- **Build real-time APIs over their streaming database** is the use case anchor—the job to be done

---

### Problem Framing

The problem framing establishes why the status quo doesn't work.

> Streaming data to UIs and AI agents requires **building and managing custom WebSockets infrastructure** [problem].

---

### Value Framing

The value framing shows how the product solves the problem. This is the main value statement.

> tycostream lets **developers** [persona] **expose streaming database views as real-time APIs without any code** [value].

---

### Supporting Arguments

Supporting arguments are the value statements and key features that back up the main value proposition. There are three of them.

---

#### 1. Subscriptions

> Unlike **custom infrastructure** [category] where you implement last-mile filtering and WebSocket delivery yourself, tycostream provides **Hasura-style filters** [feature] and **WebSocket subscriptions** [feature] out of the box.

---

#### 2. Events

> Unlike **custom infrastructure** [category] where you wire up event handling yourself, tycostream lets you define **trigger conditions** [feature] that fire **webhooks** [feature] when data changes.

---

#### 3. Configuration, Not Code

> Unlike **custom infrastructure** [category] that requires writing and maintaining code, tycostream uses **YAML configuration** [feature] to produce **typed GraphQL APIs** [feature] automatically.
