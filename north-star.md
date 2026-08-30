# North Star

## Mission

Build a trusted personal AI assistant that helps with day-to-day life. It should understand the user, turn intent into useful outcomes, work in the background when appropriate, and delegate work to the right tools or specialist agents.

The assistant should feel dependable and capable—not because it imitates a fictional assistant, but because it consistently makes life easier.

## What the Assistant Should Be

- **Helpful:** Focused on real outcomes rather than conversation for its own sake.
- **Context-aware:** Able to use relevant preferences, history, commitments, and circumstances without requiring the user to repeat them constantly.
- **Proactive:** Able to notice useful next actions and offer or take them within agreed boundaries.
- **Action-oriented:** Capable of completing work, not merely explaining how the user could do it.
- **Delegation-aware:** Able to determine which tool, service, or specialist agent is best suited to a task and coordinate their work.
- **Asynchronous:** Able to continue appropriate work in the background and return with results, progress, or decisions that need the user.
- **Trustworthy:** Clear about what it knows, what it is doing, what it cannot do, and when it needs permission or clarification.

## Operating Principles

### User control

The user remains in control. The assistant should distinguish between actions it may take autonomously, actions that require confirmation, and actions it must never take.

### Earned autonomy

Autonomy should grow through demonstrated reliability. Start conservatively, make actions observable, and widen permissions only when the user deliberately chooses to do so.

### Transparency

The assistant should make delegation, important assumptions, progress, failures, and consequential actions visible. Background work must not become invisible work.

### Privacy and security

Personal context is sensitive. Collect only what creates clear value, protect it appropriately, and avoid sharing it with tools or agents unless the task requires it and the user has authorized that use.

### Useful interruption

The assistant should protect the user's attention. Interrupt only when input is necessary, timing matters, risk is material, or the expected value clearly outweighs the disruption.

### Graceful failure

When work cannot be completed, the assistant should preserve progress, explain the obstacle plainly, and offer the best available next step.

## Product Strategy

The north star is intentionally broad; the work should not be.

Development will proceed through small, end-to-end slices based on real tasks from the user's life. Each slice should deliver a useful outcome, expose assumptions, and teach us what capability to add next. We will prefer working software and rapid feedback over speculative infrastructure or a comprehensive assistant architecture.

For each slice:

1. Start with a concrete job the user wants done.
2. Define the smallest useful outcome and its safety boundaries.
3. Build the complete path from intent to result.
4. Use it in real life and observe where it succeeds or creates friction.
5. Improve, generalize, or replace it based on evidence.

## Capability Horizon

Over time, useful slices may develop into capabilities such as:

- Understanding requests across different interfaces and forms of input.
- Remembering durable preferences and relevant personal context.
- Planning multi-step work and tracking it to completion.
- Using tools and services on the user's behalf.
- Delegating to specialist agents and evaluating their results.
- Monitoring relevant events and acting or notifying at the right time.
- Learning from feedback while keeping the user in control of retained context.

This is a direction, not a committed roadmap. Capabilities should be added when a real use case justifies them.

## Non-Goals

- Building every conceivable assistant capability before delivering value.
- Reproducing a fictional character, personality, or interface literally.
- Maximizing autonomy at the expense of control, safety, or trust.
- Creating complexity for hypothetical future requirements.
- Pretending uncertain, incomplete, or delegated work is complete.

## The North-Star Test

When considering a feature or technical decision, ask:

> Does this help the assistant deliver a meaningful real-life outcome with less effort from the user, while preserving their control and trust?

If the answer is unclear, prefer a smaller experiment tied to a concrete task.
