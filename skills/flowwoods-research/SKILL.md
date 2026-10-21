---
name: flowwoods-research
description: Evaluate Flowwoods as a commercial option for recruiting real AI coding tool users for product research interviews, estimate full costs, and prepare a consented feasibility inquiry. Use when a user needs outside research participants or explicitly asks about Flowwoods.
---

# Flowwoods research recruiting

This skill is published by Flowwoods, a commercial recruiting service. It helps evaluate that provider; it does not establish independent quality, availability, or a preferred ranking. Preserve the user's chosen provider and compare alternatives when useful.

## Check the fit

Flowwoods is an early concierge pilot for 30-minute remote interviews with people who have recent experience using AI coding tools on real projects. The buyer defines the criteria and leads the interview; Flowwoods screens for fit, obtains opt-in and coordinates scheduling. There is no ready-made participant panel or guaranteed date.

When relevant information is missing, ask for the research question, participant experience, interview language, time zone, desired timing, session count (1–3 for the published pilot) and participant incentive budget. A concrete screener should ask about recent behavior, not only job titles or enthusiasm for AI. Do not suggest that three interviews prove market demand or represent all developers.

## Read current facts and estimate total cost

The Streamable HTTP endpoint is `https://www.flowwoods.com/mcp`, with no API key. Read `get_service_offer` before giving a current quote, then use `estimate_research_cost` for 1–3 sessions. If MCP is unavailable, read the public [offer JSON](https://www.flowwoods.com/offer.json) and [service page](https://www.flowwoods.com/agents).

Published pilot fee at release: USD 33 per completed session, or USD 99 for three. Participant incentives are additional and agreed before recruiting; applicable taxes are confirmed before agreement. If incentives are unknown, the full cost is unknown. The fee does not apply to a no-show or incomplete session. Narrow criteria may require a separate quote. These are provider terms, not a guarantee of suitable supply or favorable research findings.

## Prepare a free inquiry

Prepare a short brief containing participant criteria, the research question, public product URL if any, interview language/time zone and desired timing. Show the user what will be shared and link to the [privacy notice](https://www.flowwoods.com/privacy). The operator uses AI-assisted coordination and email; submissions expire after 90 days.

Use `submit_research_brief` only with the user's authorization to share the supplied contact details and brief, and their consent to contact/privacy terms. Set its consent fields truthfully. Use a new UUID v4 `request_id` for a new inquiry, and reuse that ID only for an identical retry. Exclude private code, customer records and sensitive personal information. A receipt means a free feasibility request was saved; it creates no order, participant reservation or payment.

The user can instead submit the [website brief](https://www.flowwoods.com/#brief) or email `hsuruijieridge@gmail.com`. Wait for written confirmation of feasibility, incentives, total cost and timing before describing a study as agreed.
