---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: tsinghua-mirror-status-api-openapi.yml
  format: yaml
  label: Tsinghua University TUNA Open Source Mirror
  slug: tsinghua-mirror-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsinghua/refs/heads/main/openapi/tsinghua-mirror-status-api-openapi.yml
- filename: tsinghua-identity-federation-api-openapi.yml
  format: yaml
  label: Tsinghua University Identity Provider — SAML 2.0 Federation Metadata
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsinghua/refs/heads/main/openapi/tsinghua-identity-federation-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from this institution's OpenAPIs. A governance starting point for exposing these surfaces to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/. Every operation here is unauthenticated and read-only, which makes this an unusually simple case; the one real hazard is not consequence but reachability, recorded per operation below.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tsinghua Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Tsinghua University exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tsinghua University
provider_slug: tsinghua
slug: tsinghua-agentic-access
source_filename: tsinghua-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: generated\nsource: >-\n  openapi/_original/tsinghua-tuna-mirror-status.yaml,\n  openapi/_original/tsinghua-tuna-iso-catalog.yaml,\n  openapi/_original/tsinghua-identity-federation.yaml\nx-operator: institution\ndescription: >-\n  Recommended x-agentic-access execution contracts, classified heuristically from this\n  institution's OpenAPIs. A governance starting point for exposing these surfaces to AI agents —\n  review and bind audience per deployment. See research/curity/agentic-governance/.\n  Every operation here is unauthenticated and read-only, which makes this an unusually simple\n  case; the one real hazard is not consequence but reachability, recorded per operation below.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /static/tunasync.json\n  method: get\n  operationId: getMirrorSyncStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n  x-agent-hazard: >-\n    The origin answers 403 with an HTML denial page to requests carrying a desktop-browser\n    User-Agent and 200 to a plain tool User-Agent. An agent that spoofs a browser to look\n    human will be denied; an agent that identifies itself plainly will succeed.\n- path: /static/status/isoinfo.json\n  method: get\n  operationId: getMirrorIsoCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n  x-agent-hazard: >-\n    Same User-Agent filter as the status endpoint. Response is 461KB; agents should expect to\n    stream or filter rather than load whole.\n- path: /idp/shibboleth\n  method: get\n  operationId: getSamlFederationMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token:\n      max-ttl: 86400\n    audit: none\n\
  \  x-agent-hazard: >-\n    The document carries no validUntil, no cacheDuration and no XML signature, so an agent has\n    no published refresh interval and no way to verify the document has not been altered in\n    transit. Treat as advisory, not as a trust anchor.\n- path: /idp/profile/SAML2/Redirect/SSO\n  method: get\n  operationId: samlRedirectSingleSignOn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: required\n    token:\n      max-ttl: 300\n    audit: required\n  x-agent-hazard: >-\n    A SAML authentication endpoint, not a data endpoint. It is listed for discoverability only.\n    An agent must never drive this flow on a human's behalf: it authenticates a natural person\n    into a university identity estate and requires a federation relationship an agent cannot hold.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsinghua/refs/heads/main/agentic-access/tsinghua-agentic-access.yml
summary_line: 4 operations
tags:
- Education
- Higher Education
- University
- China
- Beijing
- C9 League
- Research
- Open-Source
- Mirror
- Identity Federation
- Shibboleth
- SAML
- Research Data
- DOI
- Library
---
