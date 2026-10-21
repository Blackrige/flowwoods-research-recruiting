# Flowwoods Research Recruiting — Agent Access

Recruit people with recent AI coding tool experience for 30-minute product research interviews. This public integration package connects to the Flowwoods hosted service. It contains configuration and a skill; it does not contain the service backend or a participant database.

**Commercial disclosure:** published by Flowwoods. This is an early concierge pilot with no ready participant panel or published paid-customer outcomes. Availability is checked for each study. The buyer runs the interviews.

## Cost and next step

- Recruiting fee: **USD 33 per completed 30-minute session**, or USD 99 for three.
- Participant incentives are separate; taxes, full cost, timing and feasibility are agreed before a study.
- Reading the offer, estimating cost and submitting a feasibility inquiry are free. No automatic charge, order or reservation.
- [Check a study's fit](https://www.flowwoods.com/#brief) · [Current scope and pricing](https://www.flowwoods.com/offer.json) · [Privacy](https://www.flowwoods.com/privacy).

## Connect over MCP

Direct Streamable HTTP endpoint, no authentication:

```text
https://www.flowwoods.com/mcp
```

For MCP clients that accept a URL configuration, see [mcp-config.json](mcp-config.json). Merge only the named entry into your own client settings.

Tools:

| Tool | Effect |
| --- | --- |
| `get_service_offer` | Read current provider scope, price and limits. |
| `estimate_research_cost` | Read-only estimate for 1–3 sessions. Missing incentives leave the total unknown. |
| `submit_research_brief` | Shares the supplied brief/contact with the operator after user authorization and privacy/contact consent. Free inquiry only. |

The write tool requires a UUID v4 for retry safety. Reuse it only for an identical retry. Do not submit personal information merely to test the integration.

## Gemini CLI extension

Unzip this package, inspect `gemini-extension.json` and the skill, then install the local folder using the Gemini CLI extension install command:

```sh
gemini extensions install /absolute/path/to/flowwoods-research
```

The manifest connects to the public endpoint and exposes the three tools above. There are no hooks, local executable helpers, API keys or automatic purchase tools. The included skill is in `skills/flowwoods-research/SKILL.md`.

## Other skill-compatible agents

Read [skills/flowwoods-research/SKILL.md](skills/flowwoods-research/SKILL.md), then use your agent's documented skill installation workflow if you want it available. Installing is optional: the public [agent page](https://www.flowwoods.com/agents) provides the same service facts.

## License and support

This integration package is MIT licensed. The license does not grant access to private service software, participant data or trademarks, and does not change the paid service terms. Contact: hsuruijieridge@gmail.com.
