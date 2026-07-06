# Style Guide

## Purpose

This document defines the writing, formatting, and quality standards for the OT/ICS Cybersecurity Roadmap.

The goal is to maintain consistency across all documentation and ensure that every page provides accurate, practical, and accessible learning material.

All contributors are expected to follow these guidelines.

---

# Core Principles

Every document in this repository should be:

* Accurate
* Clear
* Practical
* Vendor-neutral
* Beginner-friendly
* Technically correct
* Easy to maintain

Avoid unnecessary complexity. Explain concepts clearly without sacrificing technical accuracy.

---

# Writing Style

Write in a professional, instructional tone.

Use:

* Clear and concise language
* Active voice whenever possible
* Short paragraphs
* Descriptive headings
* Consistent terminology

Avoid:

* Marketing language
* Clickbait titles
* Excessive enthusiasm
* Slang
* Emojis
* AI-generated filler
* Personal opinions presented as facts

---

# Audience

Assume the reader:

* Is motivated to learn.
* Has basic computer literacy.
* May have little or no OT experience.
* Wants practical knowledge.

Never assume prior knowledge unless the module explicitly lists it as a prerequisite.

---

# Document Structure

Every learning module should follow this structure.

```text
# Title

## Overview

## Learning Objectives

## Prerequisites

## Estimated Study Time

## Core Concepts

## Required Resources

## Optional Resources

## Hands-on Labs

## Projects

## Self-Assessment

## Interview Questions

## Further Reading

## References

## What's Next
```

Supporting documents (such as policies or reference material) may use a different structure where appropriate.

---

# Learning Objectives

Learning objectives should describe measurable outcomes.

Good examples:

* Explain the Purdue Enterprise Reference Architecture.
* Configure a basic VLAN.
* Capture and analyze Modbus TCP traffic.
* Identify the components of a SCADA system.

Avoid vague objectives such as:

* Understand networking.
* Learn Linux.
* Know cybersecurity.

---

# Formatting Standards

## Headings

Use logical heading levels.

```text
# Module

## Section

### Subsection
```

Do not skip heading levels.

---

## Lists

Use unordered lists for concepts.

Example:

* PLC
* RTU
* HMI
* SCADA

Use numbered lists for procedures.

Example:

1. Install Wireshark.
2. Capture traffic.
3. Analyze packets.

---

## Tables

Use tables when comparing concepts.

Example:

| PLC           | RTU            |
| ------------- | -------------- |
| Local Control | Remote Control |

Avoid tables for simple lists.

---

## Code Blocks

Always specify the language when possible.

Example:

````text
```bash
ip addr show
```
````

---

# Terminology

Define abbreviations on first use.

Example:

> Industrial Control System (ICS)

Subsequent references may use:

> ICS

Use consistent terminology throughout the repository.

Do not alternate between different names for the same concept.

---

# Vendor Neutrality

Teach concepts before products.

Preferred approach:

* Explain PLCs before Siemens PLCs.
* Explain historians before OSIsoft PI.
* Explain industrial firewalls before vendor implementations.

Vendor examples should support the concept, not replace it.

---

# Resource Policy

Prioritize resources in the following order:

1. Official standards
2. Official documentation
3. Vendor documentation
4. Books
5. Conference presentations
6. Academic papers
7. Community resources
8. Videos

Avoid relying exclusively on YouTube or blog posts.

---

# External Links

Every external resource should include:

* Title
* Organization or Author
* URL
* Brief description
* Reason for inclusion

Example:

**NIST SP 800-82 Rev. 3**

Organization: National Institute of Standards and Technology (NIST)

Purpose:

Provides guidance for securing Industrial Control Systems.

---

# Images and Diagrams

Use diagrams only when they improve understanding.

Preferred sources:

* Original diagrams
* Official documentation
* Openly licensed content

Every image should include:

* Caption
* Source
* License (where applicable)

Avoid screenshots unless they are necessary for a lab or tutorial.

---

# Labs

Every lab should include:

* Objective
* Prerequisites
* Required software
* Estimated time
* Step-by-step instructions
* Expected outcome
* Cleanup steps
* Further challenges

Learners should be able to reproduce the lab independently.

---

# Projects

Every project should define:

* Goal
* Skills developed
* Prerequisites
* Deliverables
* Suggested tools
* Completion criteria

Projects should produce portfolio-worthy work whenever possible.

---

# Self-Assessment

Every module should conclude with review questions.

Questions should test understanding rather than memorization.

Example:

* Why is availability prioritized over confidentiality in many OT environments?
* How does Modbus TCP differ from Modbus RTU?
* What risks arise from flat industrial networks?

---

# References

Whenever possible, reference:

* Official documentation
* Industry standards
* Technical papers
* Vendor manuals
* Peer-reviewed research

Avoid unsupported technical claims.

---

# File Naming

Use lowercase filenames with hyphens.

Examples:

```text
industrial-networking.md
incident-response.md
learning-paths.md
```

Avoid:

```text
IndustrialNetworking.md
ICSNotes.md
FinalVersion2.md
```

---

# Directory Structure

Group related content together.

Example:

```text
curriculum/
labs/
projects/
resources/
standards/
certifications/
career/
```

Do not duplicate content across multiple files.

Use internal links instead.

---

# Contribution Standards

Before submitting a contribution, verify that:

* The information is technically accurate.
* Official sources have been referenced where appropriate.
* Markdown formatting is consistent.
* Internal links function correctly.
* Grammar and spelling have been reviewed.
* The content adds educational value.
* Duplicate information has been avoided.

---

# Repository Philosophy

This project prioritizes quality over quantity.

A concise, well-researched module is more valuable than a long document with outdated or inaccurate information.

Every contribution should improve the learner's understanding and move them closer to practical competence in OT/ICS cybersecurity.
