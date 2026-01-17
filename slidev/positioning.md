---
theme: default
title: tycostream positioning
colorSchema: light
transition: none
mdc: true
layout: cover
---

# tycostream positioning

How to talk about tycostream

---
layout: title-footer
---

:: title ::

# Positioning Framework

The positioning framework has 6 parts. Each part uses anchors to ground the message in something the audience already knows.

:: default ::

<Grid :items="[
  { title: 'Functional description', description: 'What is the product, who is it for, and what does it do' },
  { title: 'Problem framing', description: 'The core challenge the product solves' },
  { title: 'Value framing', description: 'The outcome and benefit the product delivers' },
  { title: 'Supporting argument 1', description: 'First proof point with features' },
  { title: 'Supporting argument 2', description: 'Second proof point with features' },
  { title: 'Supporting argument 3', description: 'Third proof point with features' }
]" :columns="3" />

:: footer ::

<Legend :items="[
  { label: 'Category', type: 'hl-category' },
  { label: 'Persona', type: 'hl-persona' },
  { label: 'Use Case', type: 'hl-usecase' },
  { label: 'Alternative', type: 'hl-alternative' },
  { label: 'Problem', type: 'hl-problem' },
  { label: 'Feature', type: 'hl-feature' },
  { label: 'Value', type: 'hl-value' }
]" />

---
layout: title-footer
---

:: title ::

# Functional Description

What is the product, who is it for, and what does it do

:: default ::

## tycostream is a [GraphQL server]{.hl-category} that helps [backend developers]{.hl-persona} [build real-time APIs over their streaming database]{.hl-usecase}.

:: footer ::

<Legend :items="[
  { label: 'Category', type: 'hl-category' },
  { label: 'Persona', type: 'hl-persona' },
  { label: 'Use Case', type: 'hl-usecase' }
]" />

---
layout: title-footer
---

:: title ::

# Problem Framing

The core challenge the product solves

:: default ::

## Streaming data to UIs and AI agents requires [building and managing custom WebSockets infrastructure]{.hl-alternative}.

:: footer ::

<Legend :items="[
  { label: 'Alternative', type: 'hl-alternative' }
]" />

---
layout: title-footer
---

:: title ::

# Value Framing

The outcome and benefit the product delivers

:: default ::

## tycostream lets [developers]{.hl-persona} [expose streaming database views as real-time APIs without any code]{.hl-value}.

:: footer ::

<Legend :items="[
  { label: 'Persona', type: 'hl-persona' },
  { label: 'Value', type: 'hl-value' }
]" />

---
layout: title-footer
---

:: title ::

# Supporting Argument 1

First proof point with features

:: default ::

## [Subscriptions]{.hl-value}

Unlike [custom infrastructure]{.hl-alternative} where you implement last-mile filtering and WebSocket delivery yourself, tycostream provides [Hasura-style filters]{.hl-feature} and [WebSocket subscriptions]{.hl-feature} out of the box.

:: footer ::

<Legend :items="[
  { label: 'Value', type: 'hl-value' },
  { label: 'Alternative', type: 'hl-alternative' },
  { label: 'Feature', type: 'hl-feature' }
]" />

---
layout: title-footer
---

:: title ::

# Supporting Argument 2

Second proof point with features

:: default ::

## [Events]{.hl-value}

Unlike [custom infrastructure]{.hl-alternative} where you wire up event handling yourself, tycostream lets you define [trigger conditions]{.hl-feature} that fire [webhooks]{.hl-feature} when data changes.

:: footer ::

<Legend :items="[
  { label: 'Value', type: 'hl-value' },
  { label: 'Alternative', type: 'hl-alternative' },
  { label: 'Feature', type: 'hl-feature' }
]" />

---
layout: title-footer
---

:: title ::

# Supporting Argument 3

Third proof point with features

:: default ::

## [Configuration, Not Code]{.hl-value}

Unlike [custom infrastructure]{.hl-alternative} that requires writing and maintaining code, tycostream uses [YAML configuration]{.hl-feature} to produce [typed GraphQL APIs]{.hl-feature} automatically.

:: footer ::

<Legend :items="[
  { label: 'Value', type: 'hl-value' },
  { label: 'Alternative', type: 'hl-alternative' },
  { label: 'Feature', type: 'hl-feature' }
]" />

---
layout: end
---

# Thank You
