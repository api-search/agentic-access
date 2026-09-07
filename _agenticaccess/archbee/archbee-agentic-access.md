---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 5
api_specs:
- filename: archbee-public-api-openapi.yml
  format: yaml
  label: Archbee Public API
  slug: archbee-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-public-api-openapi.yml
consequence_counts:
  read: 5
  write: 19
description: 'Recommended x-agentic-access execution contracts, classified from the Archbee Public API contract. Regenerated 2026-09-04: the previous version was classified against a fabricated scaffold spec describing operations Archbee does not ship (/spaces, /spaces/{spaceId}/pages). human-in-the-loop is set to required, not conditional, on the six operations whose effects Archbee documents as permanent — the API has no idempotency key, no dry-run mode and no reversal operation, so an agent cannot rehearse or undo any of them. A governance starting point; review and bind audience per deployment.'
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Archbee Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Archbee exposes 24 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 19 write.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Archbee
provider_slug: archbee
slug: archbee-agentic-access
source_filename: archbee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: generated\nsource: openapi/archbee-public-api-openapi.yml\ndescription: 'Recommended x-agentic-access execution contracts, classified from the Archbee Public API\n  contract. Regenerated 2026-09-04: the previous version was classified against a fabricated scaffold\n  spec describing operations Archbee does not ship (/spaces, /spaces/{spaceId}/pages). human-in-the-loop\n  is set to required, not conditional, on the six operations whose effects Archbee documents as permanent\n  — the API has no idempotency key, no dry-run mode and no reversal operation, so an agent cannot rehearse\n  or undo any of them. A governance starting point; review and bind audience per deployment.'\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 5\n    acting: 19\n  by_consequence:\n    read: 5\n    write: 19\n  human_in_the_loop_required: 6\noperations:\n- path: /access-control/request\n  method: post\n  operationId: requestMagicLinkAccess\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /doc\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - destructive\n      - irreversible\n    audit: required\n    reversible: false\n- path: /doc\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doc\n  method: post\n  operationId: updateCreateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /docs/search\n  method: post\n  operationId: searchDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /file-manager/file\n  method: delete\n  operationId: deleteAFileManagerFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - destructive\n      - irreversible\n    audit: required\n    reversible: false\n- path:\
  \ /file-manager/files\n  method: get\n  operationId: listFileManagerFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file-manager/move\n  method: post\n  operationId: moveAFileManagerFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /file-manager/replace\n  method: post\n  operationId: overwriteAFileManagerFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - destructive\n      - irreversible\n    audit: required\n    reversible: false\n\
  - path: /import-content\n  method: post\n  operationId: importContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /info-api-reference\n  method: get\n  operationId: infoOpenApiDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /space-group/create\n  method: post\n  operationId: createSpaceGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path:\
  \ /space-group/delete\n  method: delete\n  operationId: deleteSpaceGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - destructive\n      - irreversible\n    audit: required\n    reversible: false\n- path: /space/clone\n  method: post\n  operationId: cloneSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /space/create\n  method: post\n  operationId: createSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /space/delete\n  method: delete\n  operationId: deleteSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - destructive\n      - irreversible\n    audit: required\n    reversible: false\n- path: /space/publish\n  method: post\n  operationId: publishSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /space/update\n  method: post\n  operationId: updateSpace\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /suggest-change/discard\n  method: post\n  operationId: discardSuggestionDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - destructive\n      - irreversible\n    audit: required\n    reversible: false\n- path: /suggest-change/merge\n  method: post\n  operationId: mergeSuggestionIntoMainDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n    reversible: not-documented\n- path: /sync-api-reference\n  method: post\n  operationId: syncOpenApiDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n- path: /team/display-rules\n  method: get\n  operationId: organizationDisplayRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/export\n  method: get\n  operationId: organizationExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upload/file\n  method: post\n  operationId: uploadSingleFile\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    reversible: not-documented\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/agentic-access/archbee-agentic-access.yml
summary_line: 24 operations · 19 acting · 6 human-in-the-loop
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
- Developer Portal
- Docs as Code
- OpenAPI
- Model Context Protocol
- AI Agents
- Content Management
---
