---
title: "Understanding the Relationship Between Triggering Events, Functional Users, and Functional Processes in COSMIC"
date: 2026-08-01
permalink: /posts/triggering-events-functional-users-functional-processes-cosmic/
tags:
  - COSMIC
  - Software Measurement
  - Functional Size Measurement
---

COSMIC Measurement Manual Version 5.0 describes and explains the relationships among triggering events, functional users, and data groups. Understanding these concepts is particularly useful when identifying functional processes.

## Functional Users and Data Groups

Let us begin with two relatively familiar concepts: **functional users** and **data groups**.

In the COSMIC software context model, there are three main elements: functional users, the software being measured, and persistent storage.

Functional users may include human users, other software components, other systems, or devices. A functional user is a sender and/or intended recipient of data associated with the functional requirements of the software being measured.

Data exchanged between a functional user and the software is conveyed in the form of **data groups**.

COSMIC defines four types of data movements:

- **Entry (E)** — moves a data group from a functional user into the software.
- **Exit (X)** — moves a data group from the software to a functional user.
- **Read (R)** — moves a data group from persistent storage into the software.
- **Write (W)** — moves a data group from the software to persistent storage.

For a functional user, therefore, only two types of data movements cross the software boundary: **Entries and Exits**.

## From a Triggering Event to a Functional Process

A functional process must be initiated. At the beginning of a functional process, a functional user sends a data group to the software through an Entry.

But what causes the functional user to initiate the functional process?

This is where the concept of a **triggering event** becomes important.

A triggering event occurs outside the functional process. The occurrence of the event causes a functional user to initiate a functional process by generating and sending a data group to the software.

The relationship can therefore be understood as a sequence:

**Triggering Event → Functional User → Triggering Entry → Functional Process**

In other words, an event occurs first. In response to that event, a functional user sends a data group through a triggering Entry, which initiates a functional process.

## Why This Relationship Matters

This relationship is particularly important when identifying functional processes.

A triggering event is an event outside the software functionality being measured. For example, it may be the receipt of an order or a monitored value reaching a certain threshold.

The functional user responds to this triggering event and sends a data group—the **triggering Entry**—to the software. This initiates the corresponding functional process.

COSMIC provides a series of examples illustrating the identification of functional processes from both business application software and real-time software perspectives.

Understanding the sequence among the triggering event, functional user, triggering Entry, and functional process can therefore help clarify where one functional process begins and how it should be identified.

## Learning COSMIC Through the Measurement Manual

When learning COSMIC functional size measurement, it is useful to repeatedly consult Version 5.0 of the COSMIC Measurement Manual.

The manual is organized into three parts:

1. **Principles, Definitions & Rules**
2. **Guidelines**
3. **Examples**

When encountering an unfamiliar COSMIC term, the *Principles, Definitions & Rules* can be used to check its formal meaning. The *Guidelines* help explain how the concepts should be understood and applied, while the *Examples* provide practical cases for reinforcing that understanding.

Memorizing terminology is not the ultimate goal. More important is understanding the measurement logic behind the method so that COSMIC can be applied appropriately across different software contexts.

---

*This article is adapted from an earlier Chinese article written by the author.*
