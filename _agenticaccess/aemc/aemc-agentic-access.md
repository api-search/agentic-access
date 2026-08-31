---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: aemc-glossary-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Glossary API
  slug: aemc-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-glossary-api-openapi.yml
- filename: aemc-rule-content-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Rule Content API
  slug: aemc-rule-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-rule-content-api-openapi.yml
- filename: aemc-rule-versions-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Rule Versions API
  slug: aemc-rule-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-rule-versions-api-openapi.yml
- filename: aemc-search-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Search API
  slug: aemc-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-search-api-openapi.yml
- filename: aemc-settings-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Settings API
  slug: aemc-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-settings-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aemc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Australian Energy Market Commission exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Australian Energy Market Commission
provider_slug: aemc
slug: aemc-agentic-access
source_filename: aemc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/aemc-energy-rules-openapi-derived.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /rules/{ruleType}/versions\n  method: get\n  operationId: listRuleVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules/{versionId}/toc\n  method: get\n  operationId: getRuleTableOfContents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules/{versionId}/chapters\n\
  \  method: get\n  operationId: listRuleChapters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules/{versionId}/content/{contentId}\n  method: get\n  operationId: getRuleContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules/{versionId}/search\n  method: get\n  operationId: searchRuleVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules/{versionId}/glossary/menu\n  method: get\n  operationId: getGlossaryMenu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules/{versionId}/glossary/by-letter/{letter}\n  method: get\n  operationId: listGlossaryTermsByLetter\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules/{versionId}/glossary/{termIdentifier}\n  method: get\n  operationId: getGlossaryTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/wa\n  method: get\n  operationId: getWaSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/agentic-access/aemc-agentic-access.yml
summary_line: 9 operations
tags:
- Energy
- Australia
- Energy Markets
- Electricity
- Gas
- Utilities
- Regulations
- Smart Metering
- Consumer Data Right
- Government
- Legal
- Rules
---
