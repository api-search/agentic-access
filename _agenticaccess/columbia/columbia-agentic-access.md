---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: columbia-locations-api-openapi.yml
  format: yaml
  label: Columbia University Locations API
  slug: columbia-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/columbia/refs/heads/main/openapi/columbia-locations-api-openapi.yml
consequence_counts: {}
description: 'What an autonomous agent can actually do with Columbia University. The answer is narrow and it is unusually well-defined: exactly one API is agent-callable end to end, and the rest of the institution''s estate is actively defended against automated clients by two different challenge products.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: probed
name: Columbia Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 0
overview: 'Columbia University exposes 0 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Columbia University
provider_slug: columbia
slug: columbia-agentic-access
source_filename: columbia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes of Columbia University hosts on 2026-08-19 with and without a browser User-Agent,\n  covering the well-known discovery paths, the agent-facing conventions and every institution-\n  operated surface found.\nprovider: Columbia University\nproviderId: columbia\ndescription: >-\n  What an autonomous agent can actually do with Columbia University. The answer is narrow and it\n  is unusually well-defined: exactly one API is agent-callable end to end, and the rest of the\n  institution's estate is actively defended against automated clients by two different\n  challenge products.\ncallable_without_human:\n- surface: columbia:library-hours\n  baseURL: https://hours.library.columbia.edu/api/v1\n  x-operator: institution\n  verdict: fully_callable\n  detail: >-\n    No credential, no registration, no click-through, no rate limit encountered. Both operations\n    return application/json with Access-Control-Allow-Origin:\
  \ * — Columbia's own source sets the\n    CORS header deliberately on exactly these two actions — so an agent can call it from a\n    browser context as well as a server. Correct 400 and 404 status codes on the error paths.\n    The one trap is the missing-parameter path, which returns HTTP 200 with an HTML body; an\n    agent that trusts the status code will store a web page as data.\n- surface: columbia:identity\n  baseURL: https://shibboleth.columbia.edu/idp/shibboleth\n  x-operator: institution\n  verdict: readable\n  detail: >-\n    SAML 2.0 metadata is served anonymously as application/xml and is machine-parseable. It is\n    readable, not actionable — an agent can learn how Columbia federates identity but cannot\n    obtain an identity.\n- surface: columbia:clio-opendata\n  baseURL: https://lito.cul.columbia.edu/extracts/ColumbiaLibraryCatalog/full/\n  x-operator: institution\n  verdict: harvestable\n  detail: >-\n    108 gzipped MARCXML files plus a deletes list, served from an\
  \ open Apache directory index\n    under CC0 1.0. An agent can enumerate and download the entire Columbia catalogue with no\n    credential. There is no manifest, no checksum file and no change feed, so an agent must diff\n    the directory listing to detect updates.\nblocked_to_agents:\n- surface: opendataservice.columbia.edu, www.cuit.columbia.edu, provost.columbia.edu, ai.columbia.edu, vergil.registrar.columbia.edu\n  x-operator: institution\n  product: Cloudflare managed challenge\n  status: 403\n  detail: >-\n    Columbia's central Drupal web estate returns a \"Just a moment...\" interstitial with HTTP 403\n    to any non-browser client, including with a full browser User-Agent and navigation headers.\n    The Open Data Service — Columbia's own developer-facing service — is inside this perimeter,\n    so an agent cannot read the documentation for the feeds it is being invited to consume.\n- surface: clio.columbia.edu, academiccommons.columbia.edu, geodata.library.columbia.edu\n  x-operator:\
  \ institution\n  product: Anubis proof-of-work challenge\n  status: 200\n  detail: >-\n    Columbia University Libraries has deployed Anubis in front of its entire Blacklight discovery\n    estate. This is the more consequential of the two because it returns HTTP 200 with the\n    challenge body, so an agent that checks only the status code records a success and ingests a\n    bot-check page. It is the direct reason the OAI-PMH endpoint could not be verified, and it\n    sits in tension with the Libraries' own CC0 bulk release of the same catalogue.\n- surface: iridl.ldeo.columbia.edu\n  x-operator: institution\n  product: login redirect\n  detail: >-\n    The IRI/LDEO Climate Data Library front page is anonymous but every data path — /SOURCES/,\n    OPeNDAP, OGC WMS GetCapabilities — 302s to /auth/login. Presence without access.\ndiscovery:\n  llms_txt:\n    status: absent\n    evidence:\n    - url: https://www.columbia.edu/llms.txt\n      status: 404\n    - url: https://library.columbia.edu/llms.txt\n\
  \      status: 404\n  ai_txt:\n    status: absent\n    evidence:\n    - url: https://www.columbia.edu/ai.txt\n      status: 404\n  well_known_api_catalog:\n    status: absent\n    evidence:\n    - url: https://hours.library.columbia.edu/.well-known/api-catalog\n      status: 404\n  security_txt:\n    status: absent\n    evidence:\n    - url: https://www.columbia.edu/.well-known/security.txt\n      status: 404\n    - url: https://library.columbia.edu/.well-known/security.txt\n      status: 404\n  robots_txt:\n    status: partial\n    detail: >-\n      hours.library.columbia.edu serves a robots.txt, but it is the stock Rails template\n      containing only the commented documentation link and no directives. www.columbia.edu and\n      library.columbia.edu both return 404 for robots.txt. So Columbia challenges agents at the\n      edge while publishing no machine-readable statement anywhere about what agents may do.\n    evidence:\n    - url: https://hours.library.columbia.edu/robots.txt\n\
  \      status: 200\n    - url: https://www.columbia.edu/robots.txt\n      status: 404\n  openapi_published: false\n  mcp_server: false\n  agent_card: false\n  agent_skills: false\nsummary:\n  fully_callable_surfaces: 1\n  readable_surfaces: 2\n  challenge_blocked_hosts: 8\n  agent_discovery_files: 0\nnotes: >-\n  The shape here is worth stating precisely because it is becoming the common institutional\n  pattern: the one thing an agent can use is a small campus-life API that nobody governs, and the\n  scholarly resources the institution most wants read are the ones sitting behind an anti-crawler\n  challenge. Columbia has taken a deliberate position on automated access at the edge and has\n  published no statement of that position anywhere a machine can read it — no llms.txt, no\n  ai.txt, no meaningful robots.txt, no terms naming a sanctioned bulk route.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/columbia/refs/heads/main/agentic-access/columbia-agentic-access.yml
summary_line: 0 operations
tags:
- University
- Higher Education
- Education
- Ivy League
- Private Research University
- United States
- New York
- Identity Federation
- Library
- Open Data
- Research Repository
- Research Data
- Course Catalog
- Campus Life
---
