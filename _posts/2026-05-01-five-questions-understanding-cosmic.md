
---
title: "Five Questions That Test Your Understanding of COSMIC Functional Size Measurement"
date: 2026-05-01
permalink: /posts/five-questions-cosmic/
tags:
  - COSMIC
  - Software Measurement
  - Functional Size Measurement
---


When delivering training on the **COSMIC Functional Size Measurement (FSM) method**, I often receive similar questions from participants.

At first glance, these questions may appear to concern specific COSMIC rules. In fact, they often go deeper: they reflect whether we really understand **what software measurement is for, what should be measured, and how measurement should be used in practice**.

Here are five questions that I frequently encounter.

Before reading my answers, try answering them yourself. Write down a few keywords for each question and see whether your reasoning covers both the COSMIC method itself and the broader purpose of software measurement.

![Eight Characteristics of COSMIC]({{ '/images/blog/five-questions-cosmic/five-questions-cosmic-01.jpg' | relative_url }})

---

## 1. Can COSMIC only be used to measure requirements?

> Our company mainly develops software. Requirements are written by our customers. Can we still use COSMIC?

COSMIC can be applied at different stages of the software life cycle.

The essential point is that COSMIC functional size measurement is based on **Functional User Requirements (FUR)**. These requirements do not have to exist in one particular document or format.

Depending on the stage of the software life cycle, information about the FUR may be derived from different artifacts, such as:

- requirements clarification records;
- software requirements specifications;
- design documentation;
- the software itself or its source code;
- user manuals; or
- software interfaces.

Therefore, the question is not simply, *“Do we have a requirements specification?”*

A more important question is:

**What is the purpose of the measurement, and at what point in the software life cycle do we need the size information?**

The appropriate source of information for identifying the FUR depends largely on that measurement purpose.

![COSMIC Software Context Model]({{ '/images/blog/five-questions-cosmic/five-questions-cosmic-06.jpg' | relative_url }})

![Generic Software Model in COSMIC]({{ '/images/blog/five-questions-cosmic/five-questions-cosmic-07.jpg' | relative_url }})

---

## 2. Our company has used its own sizing method for years. Do we need to replace it with COSMIC?

Not necessarily.

Being familiar with a sizing method does not automatically mean that the method is effective. But similarly, adopting an international standard simply because it is a standard is not sufficient justification for replacing an existing method.

A useful way to evaluate an organizational sizing method is to examine historical data.

For example, collect:

- software size data; and
- a target variable such as actual development effort.

Then investigate the relationship between them.

If the organization's existing size measure has a strong and useful relationship with the target variable, such as development effort, the method may already serve its intended purpose within that organization.

Organizations often consider replacing or improving an existing sizing approach when problems arise, such as:

- excessive subjectivity;
- inconsistent counting rules;
- poor repeatability; or
- weak relationships between measured size and the variables the organization wants to analyze or estimate.

Therefore, before introducing a new functional sizing method across an organization, it can be useful to first evaluate the existing method using actual project data and make the decision based on evidence.

![Development Effort versus Requirement Points]({{ '/images/blog/five-questions-cosmic/five-questions-cosmic-02.jpg' | relative_url }})

---

## 3. Why should we use COSMIC for functional size measurement?

COSMIC has several characteristics that make it useful as a standardized functional size measurement method.

For example, the method is designed to measure functional size from the perspective of functional user requirements and to be independent of the software implementation technology.

Its measurement principles and rules can also be learned through systematic training and measurement exercises.

When introducing COSMIC into an organization, one practical approach is to begin with a representative sample of projects rather than immediately deploying the method organization-wide.

The organization can then compare COSMIC functional size with historical variables such as actual development effort.

In many practical applications, the objective is to determine whether the measured functional size provides a useful basis for activities such as:

- effort estimation;
- productivity analysis;
- benchmarking;
- project planning; and
- process improvement.

Where necessary, organizational measurement conventions may also be established while remaining consistent with the underlying COSMIC principles.

The decision to deploy COSMIC more broadly should therefore be supported by both **measurement principles and empirical evidence from the organization's own projects**.

![COSMIC Function Points versus Actual Effort]({{ '/images/blog/five-questions-cosmic/five-questions-cosmic-03.jpg' | relative_url }})

---

## 4. Why could I understand COSMIC during training but still struggle to perform real measurements?

Learning COSMIC is somewhat like learning to drive.

Understanding the rules is necessary, but understanding the rules alone does not automatically provide enough experience to handle real situations confidently.

After formal COSMIC training, organizations normally need practical measurement exercises using their own software requirements and projects.

This may involve:

- hands-on functional size measurement;
- reviewing actual measurement cases;
- one-to-one guidance for project teams;
- resolving ambiguities in real requirements;
- collecting and validating measurement data;
- integrating measurement activities into existing organizational processes; and
- developing supporting procedures, templates, guidelines, and organizational measurement conventions.

In other words, there is an important difference between:

**knowing the COSMIC rules**

and

**being able to establish and operate a functional measurement process in an organization.**

Training is only the beginning. Practical measurement, feedback, calibration, and organizational integration complete the process.

![Three Phases for Introducing COSMIC]({{ '/images/blog/five-questions-cosmic/five-questions-cosmic-04.jpg' | relative_url }})

---

## 5. Our requirements are too vague to measure functional points. How can we use COSMIC?

This is a common issue, particularly in the early stages of software development.

The underlying purpose of software sizing is to establish a **consistent way of representing software size at the level of information currently available**.

When detailed Functional User Requirements are not yet available, it may not be possible to perform a detailed COSMIC measurement directly.

Instead, organizations can explore higher-level sizing indicators based on the available information, such as:

- requirement items;
- requirement groups;
- identified functional processes; or
- other consistently defined early-size indicators.

COSMIC also provides guidance for early or approximate functional sizing when requirements are incomplete.

The key is to select a sizing approach appropriate to the available level of requirements information and then evaluate whether the resulting size measure is useful for its intended purpose.

For example, if the objective is effort estimation, historical data can be used to investigate the relationship between the selected size indicator and actual effort.

![Development Effort versus Number of Requirements]({{ '/images/blog/five-questions-cosmic/five-questions-cosmic-05.jpg' | relative_url }})

As requirements become more detailed, the measurement can progressively move toward a more detailed COSMIC functional size expressed in **COSMIC Function Points (CFP)**.

---

## From Learning COSMIC to Applying COSMIC

These five questions actually form a useful path from understanding COSMIC to applying it in practice:

**What can be measured?**  
→ Understand Functional User Requirements and the measurement purpose.

**Should an existing sizing method be replaced?**  
→ Evaluate the method using organizational data.

**Why use COSMIC?**  
→ Understand the value of a standardized functional size measure.

**Why is training alone insufficient?**  
→ Move from knowledge of the rules to practical measurement capability.

**What if the requirements are incomplete?**  
→ Select a sizing approach appropriate to the available level of information.

If your answers to these five questions are broadly consistent with this reasoning, you have probably moved beyond simply learning COSMIC terminology and rules.

You are beginning to understand the more important question:

**how functional size measurement can actually be applied within a software organization.**

---

*This article is adapted from an earlier Chinese article written by the author.*
