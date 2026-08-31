---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: photon-agent-discovery-api-openapi.yml
  format: yaml
  label: Photon Agent discovery API
  slug: photon-agent-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-agent-discovery-api-openapi.yml
- filename: photon-newsletter-api-openapi.yml
  format: yaml
  label: Photon Newsletter API
  slug: photon-newsletter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-newsletter-api-openapi.yml
- filename: photon-onboarding-api-openapi.yml
  format: yaml
  label: Photon Onboarding API
  slug: photon-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-onboarding-api-openapi.yml
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: probed
name: Photon Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 0
overview: 'Photon exposes 0 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Photon
provider_slug: photon
slug: photon-agentic-access
source_filename: photon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live fetches of https://photonhealth.com (HTML + Markdown negotiation), /llms.txt, /.well-known/api-catalog, /site-index.json\nsummary: >-\n  Photon operates one of the most deliberate agent surfaces in the catalog. The\n  marketing host is not merely agent-tolerant - it is agent-addressed: it serves\n  a Markdown twin of every canonical page under content negotiation, advertises\n  its own machine-readable contracts through an RFC 9727 API catalog AND RFC 8288\n  Link headers on every response, declares an explicit training/inference consent\n  posture in a Content-Signal header, and publishes a written policy in llms.txt\n  stating what an agent may and may not do on a user's behalf. All of it was\n  verified by probe, unauthenticated.\ndiscovery:\n  llms_txt:\n    url: https://photonhealth.com/llms.txt\n    status: 200\n    file: llms/photon-llms.txt\n    has_agent_section: true\n  docs_llms_txt:\n    url: https://docs.photon.health/llms.txt\n\
  \    status: 200\n    file: llms/photon-docs-llms.txt\n  api_catalog:\n    url: https://photonhealth.com/.well-known/api-catalog\n    status: 200\n    spec: RFC 9727\n    content_type: application/linkset+json; profile=\"https://www.rfc-editor.org/info/rfc9727\"\n    file: well-known/photon-api-catalog.json\n  openapi:\n    url: https://photonhealth.com/openapi.json\n    status: 200\n    file: openapi/photon-website-api-openapi.json\n  site_index:\n    url: https://photonhealth.com/site-index.json\n    status: 200\n    note: 40 canonical pages, each with a Markdown alternate URL; regenerated continuously (generatedAt was minutes old at probe time).\n  onboarding_schema:\n    url: https://photonhealth.com/api/onboarding/schema\n    status: 200\n    note: Machine-readable definition of every onboarding path, step and field - the contract behind the browser funnel.\nlink_headers:\n  observed: true\n  note: >-\n    Every HTML and Markdown response carries the full discovery set as RFC 8288\n\
  \    Link headers, so an agent needs no HTML parsing to find the contracts.\n  rels:\n  - rel: api-catalog\n    href: /.well-known/api-catalog\n    type: application/linkset+json\n  - rel: service-desc\n    href: /openapi.json\n    type: application/vnd.oai.openapi+json\n  - rel: service-doc\n    href: https://docs.photon.health/docs\n    type: text/html\n  - rel: describedby\n    href: /api/onboarding/schema\n    type: application/json\n  - rel: describedby\n    href: /llms.txt\n    type: text/plain\n  - rel: llms\n    href: /llms.txt\n    type: text/plain\n  - rel: index\n    href: /site-index.json\n    type: application/json\n  - rel: alternate\n    href: /index.html.md\n    type: text/markdown\n  - rel: canonical\n    href: /\n    type: text/html\nmarkdown_twins:\n  supported: true\n  negotiation: 'Accept: text/markdown'\n  alias_convention: append .md to any page URL; /index.html.md for the homepage\n  verified:\n    url: https://photonhealth.com/\n    request_header: 'Accept: text/markdown'\n\
  \    status: 200\n    response_content_type: text/markdown; charset=utf-8\n    x_markdown_tokens: 554\n  note: >-\n    The Markdown twin is the same content as the HTML page, front-mattered with\n    title/description/url/markdown - not a stripped or substituted payload. HTML\n    remains the default for browser requests. No cloaking observed: the Markdown\n    body matched the HTML page's stated subject and carried no injected or\n    sponsored content.\nconsent_signal:\n  header: Content-Signal\n  value: ai-train=yes, search=yes, ai-input=yes\n  observed_on:\n  - https://photonhealth.com/ (Markdown response)\n  - https://photonhealth.com/site-index.json (contentSignal field)\n  interpretation: >-\n    Photon affirmatively permits AI training, search indexing, and inference-time\n    input on its public marketing content. Declared in both a response header and\n    the machine-readable site index, so the posture is discoverable either way.\nagent_policy:\n  source: https://photonhealth.com/llms.txt\n\
  \  permitted:\n  - Evaluate Photon on a user's behalf.\n  - Complete the developer sandbox onboarding path with EXPLICIT user consent.\n  restricted:\n  - verbatim: Prescriber access requires verification.\n  - verbatim: Clinic, enterprise, platform, and other production paths are sales-led or handoff-led and should expect human follow-up.\n  - note: The sandbox \"cannot send real prescriptions\" - the consequential action is fenced off from the self-serve path entirely.\n  guidance:\n  - verbatim: Start with the onboarding schema.\n  - verbatim: Resolve first-party links in this file against the current host so Vercel previews and production stay aligned.\n  assessment: >-\n    A rare example of a provider writing a consent-scoped agent policy rather\n    than a blanket allow/deny: agents get an explicit, bounded lane (free\n    sandbox, user consent required) while every irreversible or regulated\n    action - real prescribing, production access - stays behind human\n    verification.\
  \ This is the escalation boundary the agentic-access model asks\n    for, expressed in prose by the provider itself.\nmcp:\n  status: planned-not-available\n  evidence: >-\n    \"A unified MCP server for Photon is planned but not yet available. In the\n    interim, agents can call the same site endpoints used by the browser\n    onboarding funnel.\" - https://photonhealth.com/llms.txt (verbatim)\n  note: First-party confirmation that no MCP server exists; see mcp/photon-mcp.yml deployment.mode = none.\naction_classes:\n- surface: photonhealth.com website API\n  operations: [getOnboardingSchema, getOpenApiSpec, getWellKnownOpenApiSpec, getApiCatalog]\n  action_class: read\n  consequence: none\n  escalation: none\n  note: Unauthenticated discovery reads; safe for autonomous agent use.\n- surface: photonhealth.com website API\n  operations: [createOrResumeOnboardingSession, saveOnboardingStep]\n  action_class: write\n  consequence: low\n  escalation: user-consent\n  note: Creates/updates\
  \ a lead record. Photon's own policy requires explicit user consent.\n- surface: photonhealth.com website API\n  operations: [submitOnboardingSession, createNewsletterSignup]\n  action_class: write\n  consequence: medium\n  escalation: user-consent\n  note: Submits the user's identity and contact details to Photon; triggers sales or verification follow-up. Not reversible by the agent.\n- surface: Clinical API (GraphQL)\n  operations: [createPrescription, createOrder, rerouteOrder]\n  action_class: write\n  consequence: high\n  escalation: human-authorization\n  note: >-\n    Prescribing is gated on write:prescription, which is issued only to verified\n    prescribers via a user access token - not obtainable by an M2M agent. The\n    provider's strongest control, enforced in the token model rather than in\n    documentation.\ngaps:\n- The agent surface is on the MARKETING host. The Clinical API (clinical-api.photon.health) serves no llms.txt, no api-catalog and no Link headers - an agent\
  \ that starts at the API host finds none of this.\n- No agent card at either well-known path on any host.\n- No MCP server yet (provider-confirmed as planned).\n- No rate-limit signal on any surface (see rate-limits/photon-rate-limits.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/agentic-access/photon-agentic-access.yml
summary_line: 0 operations
tags:
- Healthcare
- United States
- e-Prescribing
- Pharmacy
- Prescription Routing
- GraphQL
- Clinical API
- Digital Health
- Benefit Check
- Authentication
---
