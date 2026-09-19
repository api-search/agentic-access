---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: meddra-api-openapi.yml
  format: yaml
  label: MedDRA API
  slug: meddra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/openapi/meddra-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Meddra Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Meddra exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Meddra
provider_slug: meddra
slug: meddra-agentic-access
source_filename: meddra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: generated\nsource: openapi/meddra-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance\n  starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /api/di\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note: 'Reclassified by hand: the heuristic reads POST as a mutation. This operation POSTs a query body\n      and returns dictionary data; the MedDRA\
  \ API has no write surface.'\n- path: /api/detail\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note: 'Reclassified by hand: the heuristic reads POST as a mutation. This operation POSTs a query body\n      and returns dictionary data; the MedDRA API has no write surface.'\n- path: /api/downld/{lang}/{ver}/{file}/{format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - meddraapi\n- path: /api/export\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note: 'Reclassified by hand: the heuristic reads POST as a mutation. This operation POSTs a query body\n      and returns dictionary data; the MedDRA API has no write surface.'\n- path: /api/gt\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note: 'Reclassified by hand: the heuristic reads POST as a mutation. This operation POSTs a query body\n      and returns dictionary data; the MedDRA API has no write surface.'\n- path: /api/hier\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note: 'Reclassified by hand: the heuristic reads POST as a mutation. This operation POSTs a query body\n      and returns dictionary data; the MedDRA API has no write surface.'\n- path: /api/hist/{code}/{htype}/{lang}/{rsview}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - meddraapi\n- path: /api/hist/{term}/{lang}/{rsview}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - meddraapi\n- path: /api/lang/{langt}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - meddraapi\n- path: /api/rel\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - meddraapi\n- path: /api/search\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note: 'Reclassified by hand: the heuristic reads POST as a mutation. This operation POSTs a query body\n      and returns dictionary data; the MedDRA API has no write surface.'\n- path: /api/smqa\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note: 'Reclassified by hand: the heuristic reads POST as a mutation. This operation POSTs a query body\n      and returns dictionary data; the MedDRA API has no write surface.'\n- path: /api/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - meddraapi\n- path: /api/sv\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note: 'Reclassified by hand: the heuristic reads POST as a mutation.\
  \ This operation POSTs a query body\n      and returns dictionary data; the MedDRA API has no write surface.'\n- path: /api/type\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note: 'Reclassified by hand: the heuristic reads POST as a mutation. This operation POSTs a query body\n      and returns dictionary data; the MedDRA API has no write surface.'\n- path: /api/vr\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - meddraapi\n    x-review-note:\
  \ 'Reclassified by hand: the heuristic reads POST as a mutation. This operation POSTs a query body\n      and returns dictionary data; the MedDRA API has no write surface.'\nreview:\n  reviewed: '2026-09-17'\n  by: API Evangelist enrichment pass\n  note: 'The generator classifies every POST as an acting/write operation. That is wrong for MedDRA: ten of its sixteen\n    operations are POSTs that carry a JSON query body (search terms, code lists, version pairs) and return dictionary\n    data. Nothing in this API creates, updates or deletes anything on the MSSO side, so all sixteen are reclassified\n    connected/read. The one operation that deserves extra care is GET /api/downld/... , which retrieves MedDRA distribution\n    files - the constraint there is the MedDRA licence, not a write consequence.'\n  operations_reclassified: 10\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/agentic-access/meddra-agentic-access.yml
summary_line: 16 operations
tags:
- Medical Terminology
- Pharmacovigilance
- Drug Safety
- Adverse Events
- Regulatory
- Clinical Trials
- Healthcare
- Life Sciences
- Standards
- Ontology
---
