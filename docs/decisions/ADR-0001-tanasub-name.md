# ADR-0001: Tanasub name

- Status: accepted by product owner
- Date: 2026-09-16

## Decision

The product name is **Tanasub**. The name refers to proportion, harmony, relation, resemblance, and meaningful correspondence. It represents the product's central promise: discovering and sustaining fitting connections instead of decorating generic drafts with forced metaphors.

The product family is:

- **Tanasub**: umbrella brand.
- **Tanasub Open**: the public, independently usable craft system in this repository — guidance, local baseline, schemas, validators, templates, and examples.
- **Tanasub Studio**: future hosted user experience.
- **Research-to-Resonance**: the named writing method.

## Scope

This repository is Tanasub Open. It is self-contained: it must run its documented local workflow from files committed here, without private source files, a hosted account, a network connection, or any external service.

## Compatibility

1. Shared records are defined publicly with versioned JSON Schema.
2. Closed competitor implementations are never copied. Publicly observable capabilities may become clean-room specifications.
3. Open-source intake requires an exact version, licence record, provenance, security review, and removal plan.

## Consequences

The public project gains a precise identity. Visible headings and product prose use Tanasub Open, while the machine-facing skill identifier `universal-writing-guide` stays stable so existing platform installations keep working.
