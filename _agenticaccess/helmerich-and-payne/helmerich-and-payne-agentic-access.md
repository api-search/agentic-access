---
acting_count: 0
action_class_counts:
  connected: 1
api_specs:
- filename: helmerich-and-payne-survey-validation-controller-api-openapi.yml
  format: yaml
  label: Helmerich And Payne Survey Validation Controller API
  slug: helmerich-and-payne-survey-validation-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helmerich-and-payne/refs/heads/main/openapi/helmerich-and-payne-survey-validation-controller-api-openapi.yml
consequence_counts:
  read: 1
description: Recommended x-agentic-access execution contract for the one public H&P API, classified from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Helmerich And Payne Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'Helmerich And Payne exposes 1 API operation that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Helmerich And Payne
provider_slug: helmerich-and-payne
slug: helmerich-and-payne-agentic-access
source_filename: helmerich-and-payne-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: generated\nsource: openapi/helmerich-and-payne-magvar-survey-validation.json\ndescription: >-\n  Recommended x-agentic-access execution contract for the one public H&P API, classified from the\n  OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment.\nsummary:\n  operations: 1\n  by_action_class:\n    connected: 1\n  by_consequence:\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n  - path: /uncertaintyValues\n    method: get\n    operationId: uncertaintyValuesUsingGET\n    x-agentic-access:\n      action-class: connected\n      consequence: read\n      subject: not-required\n      audience: null\n      token:\n        max-ttl: null\n        note: >-\n          No token exists. The endpoint is anonymous — there is no credential to scope, rotate or\n          time-box, which also means there is no way to revoke an agent's access short of blocking\n          it at the network\
  \ layer.\n      escalation:\n        human-in-the-loop: conditional\n        triggers:\n          - eula-acceptance\n          - high-volume\n        note: >-\n          Not a consequence trigger — the call itself is harmless. The escalation exists because\n          use is governed by a EULA the agent cannot accept on the user's behalf, and because the\n          API publishes no rate limit, so sustained agent traffic is unbounded and unattributable.\n      audit: recommended\n      decision-weight: high\n      decision-weight-note: >-\n        The call has no side effects, but its OUTPUT feeds a wellbore-placement decision. An agent\n        must present the Green/Orange/Red verdict with its thresholds and the random/systematic\n        uncertainty split intact, not a summarised \"looks fine\".\nposture:\n  read_only_surface: true\n  writes_possible: false\n  reversibility: na\n  idempotency: na\n  note: >-\n    This is about as safe a surface as an agent can be given: one stateless,\
  \ anonymous,\n    side-effect-free GET with fully enumerated inputs and documented ranges. The residual risks are\n    legal (an unaccepted EULA) and interpretive (misreporting a QC verdict), not operational.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helmerich-and-payne/refs/heads/main/agentic-access/helmerich-and-payne-agentic-access.yml
summary_line: 1 operation
tags:
- Oil and Gas
- Drilling
- Energy
- Wellbore Placement
- Directional Drilling
- Survey Management
- Geomagnetics
- Rig Automation
- Industrial
---
