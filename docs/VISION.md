# Open Agency

**Status**: project scaffold. Idea captured 2026-06-12 as a retirement project.

An open-source full media-agency replacement powered by Markdown and minimal UI. The operational counterpart to the Count of Dolomites' satirical critique — same anti-extraction logic, different output.

## Philosophy

The agency model exists because of complexity arbitrage. If the complexity is encoded in open-source software, the arbitrage collapses. This project encodes 30 years of inside knowledge about how media agencies actually work into a free toolkit that lets brands (or in-house teams, or solo operators) bypass the agency entirely.

Snake Guy posture at industry scale: no invoice, no consulting fee, no managed-services overhead. Just the software that lets anyone do the work. Brands save 15-30% on agency margins; agencies collapse faster. The contribution to the industry-funeral that's already in progress.

## Why now

The holdco model is in structural decline. Drivers (in order of severity):
- Platforms selling direct (Google/Meta), collapsing media-buying commission
- Consultancies eating strategy + tech layer
- AI eating production, analytics, and account management
- In-house brand teams pulling work back
- Creator economy and founder-led shops taking creative

An open-source agency-replacement accelerates the collapse the industry is already living through. Not a disruption — a documentation of how the work could be done by anyone with the toolkit.

## Architecture: MD + minimal UI

Everything is Markdown files in git. Static site generators render for client review. AI augments authoring. APIs handle platform integrations. No proprietary formats. No vendor lock-in.

Core principles:
- **Plain text first** — every artifact is human-readable, diffable, version-controllable
- **Minimal UI** — terminal-driven workflows, static-site review surfaces
- **AI-augmented** — content generation, audience research, report drafting
- **Brand-owned auth** — brands provide their own platform credentials; the software orchestrates, doesn't broker
- **Git as collaboration** — branches, pull requests, audit trail
- **Open source** — MIT or Apache 2.0, community-driven

## Components

Each agency function gets an MD-replaceable equivalent:

| Agency function | Open Agency artifact |
|---|---|
| Creative production | `brief.md` + AI generation pipeline |
| Media planning | `media_plan.md` + budget allocation YAML |
| Media buying | API wrappers (brands provide platform auth) |
| Analytics & reporting | CSV-to-MD report generators with templates |
| Account management | git workflow + static site for client review |
| Strategy | `brief.md` + `audience.yaml` + competitive analysis MD |
| Audience research | structured YAML + AI-assisted analysis |
| Asset management | git LFS or referenced cloud storage |
| Approvals & sign-off | git commits + reviewer assignments |
| Performance dashboards | static-site generators reading CSV/API data |

## Project scaffolding (TBD)

Directory structure once built:
```
open_agency/
├── README.md (this file)
├── MANIFESTO.md (why; positioning; industry critique)
├── ARCHITECTURE.md (technical design)
├── COMPONENTS.md (function-by-function specification)
├── templates/
│   ├── brief.md
│   ├── media_plan.md
│   ├── audience.yaml
│   └── report.md
├── pipelines/
│   ├── creative_generation/
│   ├── report_generation/
│   └── platform_apis/
└── examples/
    └── example_campaign/
```

## Relationship to the catalog

- **Count of Dolomites** = satirical side. Exposes the agency-absurdity through HR-thought-leadership parody.
- **Open Agency** = operational side. Provides the actual replacement toolkit.

Both work the same anti-extraction logic at different levels. The Count makes the system visibly absurd; Open Agency makes the system functionally obsolete.

## What this is not

- Not a startup. No commercial product, no funding round, no exit.
- Not consulting. No invoice, no engagement, no managed services.
- Not a replacement for thinking. The toolkit lowers the floor of complexity; it doesn't replace strategic judgment.
- Not for monetization. Catalog ethic applies: free distribution, no DRM, no enforcement.

## Open questions

- License: MIT or Apache 2.0?
- Platform API coverage: start with what? (Google Ads + Meta Ads + a major DSP?)
- AI provider neutrality: how to make the AI pieces swappable across providers?
- Community: solo project that ships when it ships, or invite contribution from day one?
- Naming: "Open Agency" is descriptive. Could rename if the satire-energy calls for something more catalog-coded.

## Next steps

When picking this up:
1. Write MANIFESTO.md (the structural critique + the operational alternative)
2. Sketch ARCHITECTURE.md (how the pieces fit together)
3. Build templates/brief.md as the first concrete artifact
4. Pick a first end-to-end pipeline to prototype (creative_generation is probably the easiest, highest-leverage starting point)

Father's Day target is the Count's deadline. Open Agency has no deadline. Snake Guy posture: ship when it ships.
