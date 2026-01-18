---
marp: false
theme: tycostream
paginate: false
---

<!-- _class: cover -->

# tycostream positioning

How to talk about tycostream

---

<!-- _class: title-footer -->

# Framework

The positioning framework has 6 parts

<div class="grid">
  <div class="grid-item">
    <div class="number">01</div>
    <div class="title">1. Functional description</div>
    <div class="description">What is the product, who is it for, and what does it do</div>
  </div>
  <div class="grid-item">
    <div class="number">02</div>
    <div class="title">2. Problem framing</div>
    <div class="description">The core challenge the product solves</div>
  </div>
  <div class="grid-item">
    <div class="number">03</div>
    <div class="title">3. Value framing</div>
    <div class="description">The outcome and benefit the product delivers</div>
  </div>
  <div class="grid-item">
    <div class="number">04</div>
    <div class="title">4. Supporting argument 1</div>
    <div class="description">First proof point with features</div>
  </div>
  <div class="grid-item">
    <div class="number">05</div>
    <div class="title">5. Supporting argument 2</div>
    <div class="description">Second proof point with features</div>
  </div>
  <div class="grid-item">
    <div class="number">06</div>
    <div class="title">6. Supporting argument 3</div>
    <div class="description">Third proof point with features</div>
  </div>
</div>

---

<!-- _class: title-footer -->

# Anchors

Each part uses anchors to make the message concrete and specific

- <span class="hl-category">Category</span> anchors what kind of product it is
- <span class="hl-persona">Persona</span> anchors who uses it
- <span class="hl-usecase">Use Case</span> anchors the business scenario or job to be done
- <span class="hl-alternative">Alternative</span> anchors what's broken about the status quo
- <span class="hl-feature">Feature</span> anchors what capabilities enable that
- <span class="hl-value">Value</span> anchors the business outcome

---

<!-- _class: title-footer -->

# 1. Functional Description

What is the product, who is it for, and what does it do

## tycostream is a <span class="hl-category">GraphQL server</span> that helps <span class="hl-persona">backend developers</span> <span class="hl-usecase">build real-time APIs over their streaming database</span>.

<div class="legend">
  <span class="hl-category">Category</span> · <span class="hl-persona">Persona</span> · <span class="hl-usecase">Use Case</span>
</div>

---

<!-- _class: title-footer -->

# 2. Problem Framing

The core challenge the product solves

## Streaming data to UIs and AI agents requires <span class="hl-alternative">building and managing custom WebSockets infrastructure</span>.

<div class="legend">
  <span class="hl-alternative">Alternative</span>
</div>

---

<!-- _class: title-footer -->

# 3. Value Framing

The outcome and benefit the product delivers

## tycostream lets <span class="hl-persona">developers</span> <span class="hl-value">expose streaming database views as real-time APIs without any code</span>.

<div class="legend">
  <span class="hl-persona">Persona</span> · <span class="hl-value">Value</span>
</div>

---

<!-- _class: title-footer -->

# 4. Supporting Argument 1

First proof point with features

## <span class="hl-value">Real-time Subscriptions</span>

Unlike <span class="hl-alternative">custom infrastructure</span> where you implement last-mile filtering and WebSocket delivery yourself, tycostream provides <span class="hl-feature">Hasura-style filters</span> and <span class="hl-feature">WebSocket subscriptions</span> out of the box.

<div class="legend">
  <span class="hl-value">Value</span> · <span class="hl-alternative">Alternative</span> · <span class="hl-feature">Feature</span>
</div>

---

<!-- _class: title-footer -->

# 5. Supporting Argument 2

Second proof point with features

## <span class="hl-value">Event Triggers</span>

Unlike <span class="hl-alternative">custom infrastructure</span> where you wire up event handling yourself, tycostream lets you define <span class="hl-feature">trigger conditions</span> that fire <span class="hl-feature">webhooks</span> when data changes.

<div class="legend">
  <span class="hl-value">Value</span> · <span class="hl-alternative">Alternative</span> · <span class="hl-feature">Feature</span>
</div>

---

<!-- _class: title-footer -->

# 6. Supporting Argument 3

Third proof point with features

## <span class="hl-value">Configuration, Not Code</span>

Unlike <span class="hl-alternative">custom infrastructure</span> that requires writing and maintaining code, tycostream uses <span class="hl-feature">YAML configuration</span> to produce <span class="hl-feature">typed GraphQL APIs</span> automatically.

<div class="legend">
  <span class="hl-value">Value</span> · <span class="hl-alternative">Alternative</span> · <span class="hl-feature">Feature</span>
</div>

---

<!-- _class: end -->

# Thank You
