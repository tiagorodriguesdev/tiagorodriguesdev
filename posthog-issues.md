# PostHog Open Issues — No PR Open (Contributor Opportunities)

> Generated: 2026-06-21
> Source: [PostHog/posthog](https://github.com/PostHog/posthog)
> Filter: `is:open is:issue -linked:pr`

**LOE Scale:** XS (<1d) · S (1–3d) · M (1–2wk) · L (2–4wk) · XL (1mo+)

**Stack:** TypeScript/React (frontend) · Python/Django (backend) · TypeScript/Node.js (plugin server) · ClickHouse (data)

---

## Bugs

| # | Issue | LOE | Language | Notes |
|---|-------|-----|----------|-------|
| [#17229](https://github.com/PostHog/posthog/issues/17229) | Allow changing type of nested properties | **S** | TypeScript | UI change in property filter component |
| [#21769](https://github.com/PostHog/posthog/issues/21769) | Bug in breakdown insights with formula mode | **S–M** | TypeScript | Query/filter logic bug in analytics |
| [#26016](https://github.com/PostHog/posthog/issues/26016) | `ssr: false` not allowed with `next/dynamic` in Server Components | **S** | TypeScript | SDK/docs fix for Next.js App Router compat |
| [#29612](https://github.com/PostHog/posthog/issues/29612) | LLM Observability ignoring image content type for OpenAI | **S–M** | Python | Ingestion/parsing fix in LLM plugin |
| [#25913](https://github.com/PostHog/posthog/issues/25913) | Data-Management page not showing incoming events | **M** | TypeScript + Python | Live events view regression |
| [#23222](https://github.com/PostHog/posthog/issues/23222) | TypeError: Cannot redefine property `adoptedStyleSheets` | **M** | TypeScript/JS | Browser compat issue in posthog-js SDK |
| [#17865](https://github.com/PostHog/posthog/issues/17865) | Session recording not working with hashed assets | **M** | TypeScript | Replay asset resolution issue |
| [#21414](https://github.com/PostHog/posthog/issues/21414) | Slack subscription screenshots cut off | **M** | Python | Headless browser rendering/screenshot sizing |
| [#22275](https://github.com/PostHog/posthog/issues/22275) | Session replay not rendering elevated z-index DOM elements | **L** | TypeScript | Deep in rrweb/replay rendering pipeline |
| [#30826](https://github.com/PostHog/posthog/issues/30826) | PostHog does not comply with accessibility standards | **XL** | TypeScript/CSS | Broad a11y audit across entire frontend |

---

## Features / Enhancements

| # | Issue | LOE | Language | Reactions |
|---|-------|-----|----------|-----------|
| [#1289](https://github.com/PostHog/posthog/issues/1289) | Add individual user filter *(good first issue)* | **S** | TypeScript | — |
| [#3031](https://github.com/PostHog/posthog/issues/3031) | Allow filtering by "Date first seen" | **S–M** | TypeScript + Python | 18 |
| [#29310](https://github.com/PostHog/posthog/issues/29310) | Surveys: show after X amount of time (delay trigger) | **S** | TypeScript | 4 |
| [#30213](https://github.com/PostHog/posthog/issues/30213) | Surveys: RTL support | **S** | TypeScript/CSS | 2 |
| [#18979](https://github.com/PostHog/posthog/issues/18979) | Surveys: clickable persons on viewed/dismissed/sent chart | **M** | TypeScript | 1 |
| [#28256](https://github.com/PostHog/posthog/issues/28256) | Surveys: follow-up completion conditions | **M** | TypeScript + Python | 16 |
| [#28255](https://github.com/PostHog/posthog/issues/28255) | Surveys: advanced event-based trigger conditions | **M** | TypeScript + Python | 5 |
| [#27387](https://github.com/PostHog/posthog/issues/27387) | Surveys: multi-language support | **M** | TypeScript | 4 |
| [#30097](https://github.com/PostHog/posthog/issues/30097) | Surveys: inline (embedded) surveys instead of popups | **M** | TypeScript | 6 |
| [#17816](https://github.com/PostHog/posthog/issues/17816) | Email notifications for survey responses | **M** | Python | 2 |
| [#21071](https://github.com/PostHog/posthog/issues/21071) | Send surveys via email | **L** | Python + TypeScript | 21 |
| [#19031](https://github.com/PostHog/posthog/issues/19031) | Surveys: behavioral cohort targeting | **L** | Python + TypeScript | 9 |
| [#14796](https://github.com/PostHog/posthog/issues/14796) | Feature flags based on events / behavioral cohorts | **L** | Python + TypeScript | 23 |
| [#17031](https://github.com/PostHog/posthog/issues/17031) | Event retention: delete events after a timeframe | **L** | Python + ClickHouse SQL | 42 |
| [#19468](https://github.com/PostHog/posthog/issues/19468) | Event deletion | **L** | Python + ClickHouse SQL | 38 |

---

## Elixir (posthog-elixir SDK)

> Repo: [PostHog/posthog-elixir](https://github.com/PostHog/posthog-elixir)

| # | Issue | LOE | Language | Notes |
|---|-------|-----|----------|-------|
| [#29](https://github.com/PostHog/posthog-elixir/issues/29) | Telemetry integrations for Phoenix and Phoenix LiveView | **M** | Elixir | Use Phoenix/LiveView telemetry events to auto-capture page_view etc. 4 reactions. |
| [#66](https://github.com/PostHog/posthog-elixir/issues/66) | Autocapture for Phoenix LiveView | **M** | Elixir | `on_mount` hook to auto-capture `handle_event/3` calls. Issue has full working code proposal. |
| [#78](https://github.com/PostHog/posthog-elixir/issues/78) | Log support for Elixir SDK | **M–L** | Elixir | Integrate PostHog Logs product natively (currently requires manual OTel setup). |

### Cross-SDK issues that include Elixir (main repo)

| # | Issue | LOE | Language | Notes |
|---|-------|-----|----------|-------|
| [#635](https://github.com/PostHog/posthog/issues/635) | Add `page` function to all libraries *(good first issue)* | **S** | Elixir | Implement missing `page` capture method in the Elixir SDK. |
| [#48234](https://github.com/PostHog/posthog/issues/48234) | Normalize various behaviors across SDKs | **M** | Elixir | Align Elixir SDK behavior with other SDKs per spec. |

### Best Elixir Pick

**[#66](https://github.com/PostHog/posthog-elixir/issues/66) — Autocapture for Phoenix LiveView** is the standout: it's well-scoped, has a full working implementation proposal in the issue body, and solves a real pain point for Phoenix apps. The community member who filed it is actively looking to collaborate.

---

## Top Picks by Effort Level

### Quick Wins (S — 1–3 days)

- **[#26016](https://github.com/PostHog/posthog/issues/26016)** — Next.js SSR fix. Small, well-defined, TypeScript SDK work.
- **[#29310](https://github.com/PostHog/posthog/issues/29310)** — Surveys delay trigger. Pure TypeScript, well-scoped, clear spec in the issue.
- **[#30213](https://github.com/PostHog/posthog/issues/30213)** — Surveys RTL. Small CSS + TypeScript change, high value for international users.

### Medium Scope (M — 1–2 weeks)

- **[#28256](https://github.com/PostHog/posthog/issues/28256)** — Surveys follow-up conditions (16 reactions, clear feature spec).
- **[#3031](https://github.com/PostHog/posthog/issues/3031)** — "Date first seen" filter (18 reactions, touches both frontend and backend).

### High Impact (L — 2–4 weeks)

- **[#17031](https://github.com/PostHog/posthog/issues/17031)** — Event retention (42 reactions, requires ClickHouse expertise).
- **[#14796](https://github.com/PostHog/posthog/issues/14796)** — Feature flags on behavioral cohorts (23 reactions, architectural change).
