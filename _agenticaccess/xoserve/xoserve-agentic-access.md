---
acting_count: 0
action_class_counts:
  acting: 0
  connected: 4
api_specs:
- filename: xoserve-shipper-api-openapi.yml
  format: yaml
  label: Xoserve Shipper API
  slug: xoserve-shipper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-shipper-api-openapi.yml
- filename: xoserve-supplier-api-openapi.yml
  format: yaml
  label: Xoserve Supplier API
  slug: xoserve-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-supplier-api-openapi.yml
- filename: xoserve-meter-asset-api-v1-openapi.yml
  format: yaml
  label: Xoserve Meter Asset API v1
  slug: xoserve-meter-asset-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-meter-asset-api-v1-openapi.yml
- filename: xoserve-meter-asset-api-v2-openapi.yml
  format: yaml
  label: Xoserve Meter Asset API v2
  slug: xoserve-meter-asset-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-meter-asset-api-v2-openapi.yml
consequence_counts:
  physical: 0
  read: 4
  safety-critical: 0
  write: 0
description: 'Recommended x-agentic-access execution contracts for the Xoserve gas APIs. A governance STARTING POINT, not a provider claim — Xoserve publishes no agent access guidance. The surface is entirely read-only (four HTTP GETs, no write operation anywhere), so every operation classifies as action-class `connected` / consequence `read` with the 3600s read token ceiling and no human-in-the-loop requirement on the mechanics. The consequential caveat is NOT the HTTP verb: these reads return identifiable-premise data about GB gas consumers — address, current supplier, meter serial, consumption quantities — under a regulated access regime in which the requesting party must be an accredited industry participant and the consumer never consents. `subject` is therefore marked required and `purpose-required` is set on every operation: an agent must be able to state on whose behalf and for what regulated purpose it is querying a named MPRN. `audience` is left null to bind per deployment.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xoserve Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Xoserve exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Xoserve
provider_slug: xoserve
slug: xoserve-agentic-access
source_filename: xoserve-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: >-\n  The four operations Xoserve publishes through the Discovery API Platform portal API\n  (operationIds verified verbatim at\n  https://discoveryapiportal.correla.com/developer/apis/{api}/operations, HTTP 200, 2026-07-27),\n  classified against the Curity \"Access Intelligence\" x-agentic-access vocabulary.\ndescription: >-\n  Recommended x-agentic-access execution contracts for the Xoserve gas APIs. A governance STARTING\n  POINT, not a provider claim — Xoserve publishes no agent access guidance. The surface is entirely\n  read-only (four HTTP GETs, no write operation anywhere), so every operation classifies as\n  action-class `connected` / consequence `read` with the 3600s read token ceiling and no\n  human-in-the-loop requirement on the mechanics.\n  The consequential caveat is NOT the HTTP verb: these reads return identifiable-premise data about\n  GB gas consumers — address, current supplier, meter serial, consumption\
  \ quantities — under a\n  regulated access regime in which the requesting party must be an accredited industry participant\n  and the consumer never consents. `subject` is therefore marked required and `purpose-required` is\n  set on every operation: an agent must be able to state on whose behalf and for what regulated\n  purpose it is querying a named MPRN. `audience` is left null to bind per deployment.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n    acting: 0\n  by_consequence:\n    read: 4\n    write: 0\n    physical: 0\n    safety-critical: 0\n  human_in_the_loop_required: 0\n  purpose_required: 4\noperations:\n  - path: /\n    method: get\n    operationId: getShipper_1\n    spec: openapi/xoserve-shipper-api-openapi.yml\n    api: Xoserve Shipper API (Supply Point Quantities)\n    x-agentic-access:\n      action-class: connected\n      consequence: read\n      subject: required\n      audience: null\n      token:\n        max-ttl: 3600\n      constraints:\n  \
  \      purpose-required: true\n        data-class: identifiable-premise\n        eligibility: 'licensed GB gas Shipper; Azure APIM subscription approved by Xoserve'\n      audit: required\n      audit-reason: >-\n        Returns proposed Formula Year AQ/SOQ for a named MPRN ahead of the market notification —\n        commercially sensitive and premise-identifying.\n  - path: /\n    method: get\n    operationId: getSupplier_1\n    spec: openapi/xoserve-supplier-api-openapi.yml\n    api: Xoserve Supplier API (Supply Point Enquiry)\n    x-agentic-access:\n      action-class: connected\n      consequence: read\n      subject: required\n      audience: null\n      token:\n        max-ttl: 3600\n      constraints:\n        purpose-required: true\n        data-class: identifiable-premise\n        eligibility: 'REC party, access granted by RECCo per the REC Data Access Matrix'\n      audit: required\n      audit-reason: >-\n        89-field supply meter point record resolvable from a postcode\
  \ — including current and previous\n        supplier, latest meter read and priority-consumer indicator.\n  - path: /\n    method: get\n    operationId: getMeterAsset_1\n    spec: openapi/xoserve-meter-asset-api-v1-openapi.yml\n    api: Xoserve Meter Asset API v1\n    x-agentic-access:\n      action-class: connected\n      consequence: read\n      subject: required\n      audience: null\n      token:\n        max-ttl: 3600\n      constraints:\n        purpose-required: true\n        data-class: identifiable-premise\n        eligibility: 'REC party, access granted by RECCo per the REC Data Access Matrix'\n      audit: required\n  - path: /\n    method: get\n    operationId: getMeterAsset_1\n    spec: openapi/xoserve-meter-asset-api-v2-openapi.yml\n    api: Xoserve Meter Asset API v2\n    x-agentic-access:\n      action-class: connected\n      consequence: read\n      subject: required\n      audience: null\n      token:\n        max-ttl: 3600\n      constraints:\n        purpose-required:\
  \ true\n        data-class: identifiable-premise\n        eligibility: 'REC party, access granted by RECCo per the REC Data Access Matrix'\n      audit: required\n      audit-reason: >-\n        v2 adds full supplier / MAP / MAM change history, making bulk enumeration a switching-market\n        intelligence risk as well as a privacy one.\ndeployment_notes:\n  - >-\n    Rate governance is contractual, not technical: the annual call-allowance band (60,000–18,000,000\n    calls/year) is the real ceiling and nothing in the response signals remaining budget. Give an agent\n    a hard local quota — see rate-limits/xoserve-rate-limits.yml.\n  - >-\n    Credentials are long-lived Azure APIM subscription keys with no scopes, no expiry signal and no\n    rotation endpoint. The 3600s max-ttl above applies to any token an agent platform mints in front of\n    the key, not to the key itself, which must never be handed to a model.\n  - >-\n    Enumeration is the dominant abuse mode: postcode-based\
  \ lookup on the Shipper and Supplier APIs\n    makes address-space sweeping trivial. Constrain agents to MPRNs already in scope for the stated purpose.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/agentic-access/xoserve-agentic-access.yml
summary_line: 4 operations
tags:
- Energy
- United Kingdom
- Gas
- Utilities
- Energy Markets
- Meter Data
- Gas Networks
- Central Data Service Provider
- Data Services
---
