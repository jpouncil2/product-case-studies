# Engineering leadership and real-time systems

**Early-stage product direction, engineering teams, and high-concurrency systems**

This case study is a high-level overview of my experience leading engineering and guiding architecture. It is not a reproduction of an employer's system, repository, client materials, or internal documentation.

## Two complementary settings

| Setting | My role | What it demonstrates |
|---|---|---|
| MeApps Corporation (2014–2018) | Director of Software Engineering and Business Development | Bringing product, technical planning, delivery, and business development together in an early-stage environment |
| CBS Sports / Paramount (2020–2023) | Senior Manager, Data Engineering | Leading engineering at scale; guiding the reliability and architecture of a real-time data platform |

## The product and engineering work

**At MeApps**, my role crossed product direction, business development, and software engineering leadership. The challenge was not just choosing a technical approach; it was aligning product priorities and implementation choices with the needs of the business. This is relevant to founder-led engagements that need senior technical judgment without a large executive team.

**At CBS Sports / Paramount**, I managed approximately 20 engineers across three teams. A major part of my work included a real-time data-distribution platform serving more than one million concurrent client connections. The engineering challenge involved delivering timely updates to many connected clients while balancing concurrency, service reliability, operational recovery, and maintainability.

## How I approach architecture and teams

- **Start with outcomes and constraints.** Understand the business's latency, reliability, budget, and delivery requirements before committing to architecture.
- **Design for the actual workload.** Identify the parts of a system where connections, data distribution, and failure recovery create the main risks.
- **Review trade-offs, not just diagrams.** Evaluate latency and scaling options alongside operating cost, debugging, and staffing needs.
- **Make quality actionable.** Use engineering review, tests, deployment safeguards, and clear ownership rather than relying on architectural intent alone.
- **Build a team that can own the result.** Set responsibilities, mentor engineering leads, and translate technical risk into decisions founders and stakeholders can make.

## High-level conceptual system view

The sketch below illustrates **general concerns in a real-time pub/sub product**. It is **not** an employer architecture diagram or an exhaustive specification of a proprietary system.

```text
Event-producing services
         |
         v
  Distribution layer
         |
  +------+------+
  |             |
  v             v
Connection   Operational
services     telemetry
  |
  v
Large population of connected clients

Design questions: subscription boundaries, fan-out,
capacity planning, failure recovery, observability.
```

## Why this work matters for fractional technical leadership

I bring early-stage product and business alignment experience alongside enterprise engineering leadership. That combination helps me work with a founder on the roadmap while also reviewing the architecture, delivery process, vendor trade-offs, and scaling risks behind it.

My previous formal titles were Director of Software Engineering and Business Development and Senior Manager, Data Engineering—not Chief Technology Officer. I describe this as **CTO-relevant technical leadership experience**, not prior service in a fractional CTO title.

## Public-sharing boundaries

- No proprietary source code, internal design documents, employer screenshots, infrastructure identifiers, or client records are included.
- The illustrative diagram is intentionally generic.
- Dates and scale are presented as professional experience, without claims about proprietary implementation details.
- The portfolio's product-building case studies provide separate examples of more recent independent work, including [Roomfor Studio](../roomfor-studio/README.md).
