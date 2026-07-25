---
acting_count: 0
action_class_counts:
  connected: 33
api_specs:
- filename: chameleon-alert-groups-api-openapi.yml
  format: yaml
  label: Chameleon Alert Groups API
  slug: chameleon-alert-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-alert-groups-api-openapi.yml
- filename: chameleon-companies-api-openapi.yml
  format: yaml
  label: Chameleon Companies API
  slug: chameleon-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-companies-api-openapi.yml
- filename: chameleon-deliveries-api-openapi.yml
  format: yaml
  label: Chameleon Deliveries API
  slug: chameleon-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-deliveries-api-openapi.yml
- filename: chameleon-domains-api-openapi.yml
  format: yaml
  label: Chameleon Domains API
  slug: chameleon-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-domains-api-openapi.yml
- filename: chameleon-imports-api-openapi.yml
  format: yaml
  label: Chameleon Imports API
  slug: chameleon-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-imports-api-openapi.yml
- filename: chameleon-interactions-api-openapi.yml
  format: yaml
  label: Chameleon Interactions API
  slug: chameleon-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-interactions-api-openapi.yml
- filename: chameleon-launchers-api-openapi.yml
  format: yaml
  label: Chameleon Launchers API
  slug: chameleon-launchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-launchers-api-openapi.yml
- filename: chameleon-limit-groups-api-openapi.yml
  format: yaml
  label: Chameleon Limit Groups API
  slug: chameleon-limit-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-limit-groups-api-openapi.yml
- filename: chameleon-microsurveys-api-openapi.yml
  format: yaml
  label: Chameleon Microsurveys API
  slug: chameleon-microsurveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-microsurveys-api-openapi.yml
- filename: chameleon-profiles-api-openapi.yml
  format: yaml
  label: Chameleon Profiles API
  slug: chameleon-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-profiles-api-openapi.yml
- filename: chameleon-properties-api-openapi.yml
  format: yaml
  label: Chameleon Properties API
  slug: chameleon-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-properties-api-openapi.yml
- filename: chameleon-responses-api-openapi.yml
  format: yaml
  label: Chameleon Responses API
  slug: chameleon-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-responses-api-openapi.yml
- filename: chameleon-segments-api-openapi.yml
  format: yaml
  label: Chameleon Segments API
  slug: chameleon-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-segments-api-openapi.yml
- filename: chameleon-tags-api-openapi.yml
  format: yaml
  label: Chameleon Tags API
  slug: chameleon-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-tags-api-openapi.yml
- filename: chameleon-tooltips-api-openapi.yml
  format: yaml
  label: Chameleon Tooltips API
  slug: chameleon-tooltips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-tooltips-api-openapi.yml
- filename: chameleon-tours-api-openapi.yml
  format: yaml
  label: Chameleon Tours API
  slug: chameleon-tours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-tours-api-openapi.yml
- filename: chameleon-webhooks-api-openapi.yml
  format: yaml
  label: Chameleon Webhooks API
  slug: chameleon-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/openapi/chameleon-webhooks-api-openapi.yml
consequence_counts:
  read: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chameleon Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'Chameleon exposes 33 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chameleon
provider_slug: chameleon
slug: chameleon-agentic-access
source_filename: chameleon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chameleon-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 33\n  by_consequence:\n    read: 33\n  human_in_the_loop_required: 0\noperations:\n- path: /analyze/profiles\n  method: get\n  operationId: listProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze/profiles/{id}\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze/companies\n  method: get\n  operationId: listCompanies\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze/companies/{id}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/segments\n  method: get\n  operationId: listSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/segments/{id}\n  method: get\n  operationId: getSegment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/tours\n  method: get\n  operationId: listTours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /edit/tours/{id}\n  method: get\n  operationId: getTour\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze/interactions\n  method: get\n  operationId: listInteractions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze/interactions/{id}\n  method: get\n  operationId: getInteraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/surveys\n  method: get\n  operationId: listSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/surveys/{id}\n  method: get\n  operationId: getSurvey\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze/responses\n  method: get\n  operationId: listResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/deliveries\n  method: get\n  operationId: listDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/delivery/{id}\n  method: get\n  operationId: getDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/limit_groups\n  method: get\n  operationId: listLimitGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/limit_groups/{id}\n\
  \  method: get\n  operationId: getLimitGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/alert_groups\n  method: get\n  operationId: listAlertGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/alert_groups/{id}\n  method: get\n  operationId: getAlertGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/launchers\n  method: get\n  operationId: listLaunchers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/launchers/{id}\n  method: get\n  operationId: getLauncher\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/tooltips\n  method: get\n  operationId: listTooltips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/tooltips/{id}\n  method: get\n  operationId: getTooltip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/urls\n  method: get\n  operationId: listDomains\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/urls/{id}\n  method: get\n  operationId: getDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/properties\n  method: get\n  operationId: listProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /edit/properties/{id}\n  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/imports\n  method: get\n  operationId: listImports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/imports/{id}\n  method: get\n  operationId: getImport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chameleon/refs/heads/main/agentic-access/chameleon-agentic-access.yml
summary_line: 33 operations
tags:
- Product
- In-App Guidance
- Onboarding
- Surveys
- Analytics
---
