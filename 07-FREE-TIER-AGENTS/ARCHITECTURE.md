# VELORA Avatar AI — Free-Tier Agent Architecture (proposal)

Goal: orchestrate available free tiers without assuming any website has an automation API or permits browser bots.

## Non-negotiable
Canonical avatar IMG_7316.jpeg, OpenArt ID 5AnoW2agSbonaMWxQ8uK. Use same identity reference every time and visually QA all outputs. Official VELORA logo remains an original asset, preferably composited rather than regenerated.

## Agent roles
1. Orchestrator: plan requests, select allowed tools, track budget/credits, request approval for paid actions.
2. Avatar identity agent: build consistent reference shots, compare identity and reject drift.
3. Image agent: compare Leonardo AI, Nano Banana Pro, Ideogram, Arena where free tiers allow. Free web access != free API.
4. Video agent: compare Google Flow, OpenArt, Meta AI Vibes where free tiers permit; create short shots with shared reference.
5. Editor agent: assemble scenes, subtitles, transitions and audio using CapCut where available, or local FFmpeg (free/open-source) when suitable.
6. QA/security agent: check character identity, official logo, copyright, dimensions, durations, costs, service terms and permissions.
7. Archive agent: store prompts, references, status and approved outputs in GitHub/OpenArt subject to upload permissions.

## Candidate tools to verify
OpenArt, CapCut, Google AI Studio (Gemini), Arena.ai, Nano Banana Pro, Qven Chat AI (name/product needs verification), Leonardo AI, Ideogram AI, Meta AI Vibes, Google Flow.

## Feasibility statuses
- GitHub repository: connected; can archive textual plans.
- OpenArt: connected; video generation working, subscription currently Pro (not free).
- CapCut: desktop/mobile manual editing available as a workflow candidate; external automation not verified.
- Google AI Studio, Flow, Arena, Leonardo, Ideogram, Meta AI Vibes, Nano Banana Pro: no verified automation connection or free API quota in this project.
- Qven Chat AI: exact provider/product not yet verified.
- Autonomous agents: NOT deployed; these are architecture specifications only.

## Implementation stages
A. Verify free-tier limits, API availability and automation permission per provider.
B. Implement a simple orchestration manifest and QA checklist.
C. Connect only authorized supported APIs; route unsupported web-only tools to manual approval.
D. Pilot one 30-second VELORA ad from three 10-second shots; assemble and inspect before release.

Avoid password sharing, bypassing rate limits, automated account creation or violating service terms.
