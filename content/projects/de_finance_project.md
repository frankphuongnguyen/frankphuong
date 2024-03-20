---
title: Data Engineering Finance Project - Last Capital - 001. Overview platform
date: 2023-02-10
showtoc: true
draft: false
---

#### Propeties

Github repository: [de_finance_project](https://github.com/frankphuongnguyen/)
Tags: #finance, #dataengineering


## Introduction

Have you ever imagine how a data engineer thinking and building a data system?
Let's start with a finance project.

Suppose you are a data engineer at a finance trading services company - Last Capital, established in early 2024.
As a first member of team Data Engineering, you have a responsibility to build multiple components of company's data system. You must have ability to analysis requirements, plaining, execute, and monitoring all components.
Now, what do you do?

To be clear and more unstandable about this company, I suppose company have some overviews:

1. Last Capital's platform have multiple products and services: Open-ended fund exchange, Algorithmic trading, Market sentiment analysis.
2. Last Capital's product running on multiple platforms: Web, iOS, Android.
3. Market: Vietnam.
4. Some big challenges:
   - Collect user data using web/app: Get users to stick with the Last Capital's product.
   - Predict user's sentiment in market: Base on both news and market's transaction.
   - High freqency trading: When KRX system go-live, this function will make high impact for Last Capital because we have strong quants developers and quants researchers.

This is overview about Last Capital's platform and strategy about data. But in this post, we just focus on "Collect user data using web/app", if I have more chance, we will build anothers function later.


## Let's jump in

I think we must be clear some main requirements with most important stackholder: Founder.

Nothing be clear, both functional and non-functional requirements.
You need to have ability to get more clearly requirements as you can.
  
To be quick, I suppose I get some requirements:

- Business requirements:
- Functional requirements:
- Non-Functional requirements:

Based on define of [The Data Engineering Lifecycle]()[01], a data system have several parts:

- Generation
- Storage
- Ingestion
- Transformation
- Serving

Let's execute requirements to specific elements.

### Generation

> How data created?

Yes, "How data created?".
What is the matrix question you need to ask before doing something?

- What is the main characteristics of the datasource? Is it a application? Or devices?
- How many events created by this source by time? Total summary data we have per minitues/hour/day/... ?
- Is message error frequency? How many times? Is it acceptable or not?

Answers:

- The data generation from application on web, iOS devices, android devices.
- Total number users we have is ~5000, and the accuracy daily user active is ~75%. ()
- 


So, I think we can build system on on-premise version and cloud version.

- [[Data Engineering Finance Project - Last Capital] - 002. On-premise version]()
- [[Data Engineering Finance Project - Last Capital] - 003. Cloud version (AWS)]()


Related:

- [01][The Data Engineering Lifecycle](https://learning.oreilly.com/library/view/fundamentals-of-data/9781098108298/ch02.html)
