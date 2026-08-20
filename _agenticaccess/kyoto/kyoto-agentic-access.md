---
acting_count: 0
action_class_counts:
  connected: 21
api_specs:
- filename: kyoto-oai-pmh-api-openapi.yml
  format: yaml
  label: KURENAI OAI-PMH API
  slug: kyoto-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-oai-pmh-api-openapi.yml
- filename: kyoto-rest-api-openapi.yml
  format: yaml
  label: KURENAI DSpace REST API
  slug: kyoto-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-rest-api-openapi.yml
- filename: kyoto-lms-api-openapi.yml
  format: yaml
  label: PandA Learning Support System API (Sakai Entity Broker + IMS LTI)
  slug: kyoto-lms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-lms-api-openapi.yml
consequence_counts:
  read: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPIs in this repository. A governance starting point for exposing these surfaces to AI agents — review and bind audience per deployment. Every operation covered here is an anonymous or session-gated READ; Kyoto University publishes no write surface. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kyoto Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Kyoto University exposes 21 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kyoto University
provider_slug: kyoto
slug: kyoto-agentic-access
source_filename: kyoto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: generated\nsource: openapi/_original/kyoto-kurenai-oai.yaml, openapi/kyoto-lms-api-openapi.yml — regenerated 2026-08-19\n  when the PandA (Sakai) LMS surface was added. The previous file named a source path that did not exist\n  (openapi/kyoto-kurenai-oai.yaml).\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPIs\n  in this repository. A governance starting point for exposing these surfaces to AI agents — review and\n  bind audience per deployment. Every operation covered here is an anonymous or session-gated READ; Kyoto\n  University publishes no write surface. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 21\n  by_consequence:\n    read: 21\n  by_subject:\n    optional: 18\n    required: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /server/api\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /server/api/core/communities\n  method: get\n  operationId: listCommunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /server/api/core/communities/{uuid}\n  method: get\n  operationId: getCommunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /server/api/core/collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /server/api/core/items\n  method: get\n  operationId: listItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /server/oai/request\n  method: get\n  operationId: oaiRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/describe\n  method: get\n  operationId: describeEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/tool.json\n  method: get\n  operationId: listTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/site.json\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/syllabus.json\n  method: get\n  operationId: listSyllabus\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/announcement.json\n  method: get\n  operationId: listAnnouncements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/calendar.json\n  method: get\n  operationId: listCalendarEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/assignment.json\n  method: get\n  operationId: listAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/content.json\n  method: get\n  operationId: listContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /direct/lti.json\n  method: get\n  operationId: listLtiTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/session.json\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct/user.json\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n    note: Anonymous callers are refused (403/401/400). An agent needs a Kyoto University session, which\n      is federated through the IIMC Shibboleth IdP — treat as out of scope for unattended agents.\n- path: /direct/poll.json\n  method: get\n  operationId: listPolls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n    note: Anonymous callers are refused (403/401/400). An agent needs a Kyoto University session, which\n      is federated through the IIMC Shibboleth IdP — treat as out of scope for unattended agents.\n- path: /direct/membership.json\n  method: get\n  operationId: listMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: none\n    note: Anonymous callers are refused (403/401/400). An agent needs a Kyoto University session, which\n      is federated through the IIMC Shibboleth IdP — treat as out of scope for unattended agents.\n- path: /imsblis/lti13/keyset\n  method: get\n  operationId: getLti13Keyset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imsblis/service/\n  method: get\n  operationId: ltiBasicOutcomesService\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    note: LTI 1.1 grade passback. Reads succeed but real use is a signed POST that writes grades — do\n      not let an agent call this without a human.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/agentic-access/kyoto-agentic-access.yml
summary_line: 21 operations
tags:
- University
- Higher Education
- Education
- Japan
- National University
- Research Repository
- Research Data
- Identity Federation
- Learning Management
- Open Access
- Research Computing
- Scholarly
---
