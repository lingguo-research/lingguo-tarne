---
title: "If Management Work Cannot Be Measured in COSMIC Function Points, How Can Its Effort Be Estimated?"
date: 2026-07-01
permalink: /posts/cosmic-functional-size-and-management-effort/
tags:
  - COSMIC
  - Software Measurement
  - Software Estimation
  - Effort Estimation
---

I recently received a question from a reader about the relationship between functional size and effort:

> **Management activities are not directly associated with functional size. Should the cost of management work therefore be estimated separately?**
![Reader question about management effort](/images/blog/functional-size-effort/management-effort-question.jpg)
The question came from an organization where software development is outsourced to several suppliers. Front-end development, back-end development, and testing are performed by different teams, while project management and overall coordination are handled internally.

Different roles are typically charged according to the effort they spend on the project. The organization therefore wants to plan ahead and estimate the effort required by these different activities as accurately as possible for budgeting purposes.

They are using COSMIC functional size measurement for the front-end, back-end, and testing-related software, but they are unsure how to deal with management effort.

## COSMIC Measures Software Size, Not Management Activities

COSMIC functional size measurement measures the functional size of software based on its **Functional User Requirements (FUR)**.

Put simply:

**If there is software functionality, its functional size can potentially be measured. If there is no software functionality, there is no functional size to measure.**

Consider typical project management activities:

- organizing project meetings;
- monitoring project progress;
- coordinating among teams;
- preparing weekly reports and presentations;
- reporting project status to management.

These activities do not correspond to software functionality delivered by the project. Therefore, their functional size cannot be measured using COSMIC.

However, **having no COSMIC functional size does not mean that an activity requires no effort.**

## Functional Size and Effort Are Different Dimensions

Functional size and effort measure different characteristics of a software project.

We measure functional size partly because size can provide a useful basis for estimating effort. In this way, two different dimensions—**size** and **effort**—can be statistically related.

Importantly, this relationship does not have to be one-to-one.

For example, we do not necessarily need to use:

**development size → development effort**

or:

**testing size → testing effort**

A measured software size may also be used to estimate:

**software size → testing effort**

or even:

**software size → project management effort**

The important question is not whether the activity itself has a functional size. The important question is whether historical data show a useful relationship between software size and the effort required for that activity.

## Historical Data Provide the Mapping

When sufficient historical data have been collected, organizations can investigate relationships between functional size and many other project variables they want to estimate.

For example, functional size can potentially be related to:

- number of test cases;
- test case preparation effort;
- testing effort;
- testing rework effort;
- project management effort;
- overall project effort.

Suppose we want to estimate the number of test cases required for a project.

Writing test cases is not itself software functionality, so we cannot measure the functional size of the activity “write test cases.”

However, this does not mean that the number of test cases cannot be estimated.

If historical project data show a relationship between software functional size and the number of test cases, we can build an estimation model:

**Functional Size → Number of Test Cases**

![Relationship between functional size and number of test cases](/images/blog/functional-size-effort/functional-size-test-cases.jpg)

The same principle can be extended to effort:

**Functional Size → Test Case Preparation Effort**

**Functional Size → Testing Effort**

**Functional Size → Testing Rework Effort**

The relationship must be established and validated using historical data.

## Different Production Lines May Have Different Productivity Patterns

The same idea can be applied when analyzing productivity.

Suppose an organization maps functional size and effort for projects belonging to several different production lines. The data may reveal that each production line has a different productivity pattern.

![Productivity patterns across production lines](/images/blog/functional-size-effort/productivity-by-production-line.jpg)

This information can support management decisions.

For example, directly comparing productivity across production lines may not be appropriate because each production line may have different characteristics. Comparisons within the same production line may be more meaningful.

If one production line consistently requires more effort per unit of functional size, the organization can investigate the underlying reasons and identify opportunities for process improvement.

Conversely, if another production line consistently requires less effort, its practices can be analyzed to determine whether some of them could be adopted elsewhere in the organization.

## Conclusion

Functional size and effort are two different dimensions of software measurement. They do not have a strict one-to-one relationship.

Even when an activity cannot itself be measured in COSMIC function points, its effort may still be estimated by establishing an empirical relationship between **software functional size** and **historical data for that activity**.

A reliable functional-size baseline therefore provides much more than a measure of software size. Combined with sufficient historical data, it can become the foundation for estimating and analyzing many different aspects of software projects.

---

*This article is adapted from an earlier Chinese article written by the author.*
