# tmux for EvoCUA: Empirical Evaluation Protocol

## Purpose

This document records the research framing behind the static GitHub Pages site. The project studies how tmux can be adapted for EvoCUA as a durable terminal substrate for agentic work.

## Research Question

Which measurements reveal whether EvoCUA is using tmux as a durable workspace rather than a passive command transport?

## Working Thesis

Evaluation should measure the full interaction trace, including focus decisions, pane reuse, interruption recovery, and the stability of intermediate artifacts.

## Design Claims

- Tasks are grouped by session length and required recovery depth.
- Ablations remove pane memory, replay buffers, and focus metadata independently.
- Metrics distinguish successful task completion from reproducible terminal conduct.

## Evaluation Lens

- Long-horizon task completion
- Recovery latency after injected faults
- Agreement between trace replay and final artifacts


## Threats to Validity

- Terminal state can be over-instrumented, causing an adapter to measure artifacts of the harness rather than real agent behavior.
- A final successful artifact may hide poor recovery behavior, repeated command attempts, or fragile focus management.
- Agent-specific adapters can become difficult to compare unless trace schemas remain explicit and documented.

## Hero Image Source

The GitHub Pages hero image uses the shared tmux CUA screenshot, copied into `docs/assets/hero.png` at its original 1484x1060 PNG resolution.
