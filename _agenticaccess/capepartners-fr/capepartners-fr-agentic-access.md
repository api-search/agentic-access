---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 32
api_specs:
- filename: capepartners-fr-activity-api-openapi.yml
  format: yaml
  label: Cape Partners Activity API
  slug: capepartners-fr-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-activity-api-openapi.yml
- filename: capepartners-fr-confidentiality-api-openapi.yml
  format: yaml
  label: Cape Partners Confidentiality API
  slug: capepartners-fr-confidentiality-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-confidentiality-api-openapi.yml
- filename: capepartners-fr-dataquality-api-openapi.yml
  format: yaml
  label: Cape Partners Data Quality API
  slug: capepartners-fr-dataquality-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-dataquality-api-openapi.yml
- filename: capepartners-fr-dealflow-api-openapi.yml
  format: yaml
  label: Cape Partners Deal Flow API
  slug: capepartners-fr-dealflow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-dealflow-api-openapi.yml
- filename: capepartners-fr-discovery-api-openapi.yml
  format: yaml
  label: Cape Partners Discovery API
  slug: capepartners-fr-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-discovery-api-openapi.yml
- filename: capepartners-fr-exchange-api-openapi.yml
  format: yaml
  label: Cape Partners Exchange API
  slug: capepartners-fr-exchange-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-exchange-api-openapi.yml
- filename: capepartners-fr-identity-api-openapi.yml
  format: yaml
  label: Cape Partners Identity API
  slug: capepartners-fr-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-identity-api-openapi.yml
- filename: capepartners-fr-infomemos-api-openapi.yml
  format: yaml
  label: Cape Partners Info Memos API
  slug: capepartners-fr-infomemos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-infomemos-api-openapi.yml
- filename: capepartners-fr-interest-api-openapi.yml
  format: yaml
  label: Cape Partners Interest API
  slug: capepartners-fr-interest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-interest-api-openapi.yml
- filename: capepartners-fr-mandate-api-openapi.yml
  format: yaml
  label: Cape Partners Mandate API
  slug: capepartners-fr-mandate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-mandate-api-openapi.yml
- filename: capepartners-fr-matching-api-openapi.yml
  format: yaml
  label: Cape Partners Matching API
  slug: capepartners-fr-matching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-matching-api-openapi.yml
- filename: capepartners-fr-pairings-api-openapi.yml
  format: yaml
  label: Cape Partners Pairings API
  slug: capepartners-fr-pairings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-pairings-api-openapi.yml
- filename: capepartners-fr-registration-api-openapi.yml
  format: yaml
  label: Cape Partners Registration API
  slug: capepartners-fr-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-registration-api-openapi.yml
- filename: capepartners-fr-search-api-openapi.yml
  format: yaml
  label: Cape Partners Search API
  slug: capepartners-fr-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-search-api-openapi.yml
- filename: capepartners-fr-valuation-api-openapi.yml
  format: yaml
  label: Cape Partners Valuation API
  slug: capepartners-fr-valuation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capepartners-fr/openapi/capepartners-fr-valuation-api-openapi.yml
consequence_counts:
  physical: 1
  read: 32
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Capepartners Fr Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a/message:send
operation_count: 48
overview: 'Cape Partners exposes 48 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 15 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cape Partners
provider_slug: capepartners-fr
slug: capepartners-fr-agentic-access
source_filename: capepartners-fr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/capepartners-fr-activity-api-openapi.yml, openapi/capepartners-fr-confidentiality-api-openapi.yml,\n  openapi/capepartners-fr-dataquality-api-openapi.yml, openapi/capepartners-fr-dealflow-api-openapi.yml,\n  openapi/capepartners-fr-discovery-api-openapi.yml, openapi/capepartners-fr-exchange-api-openapi.yml,\n  openapi/capepartners-fr-identity-api-openapi.yml, openapi/capepartners-fr-infomemos-api-openapi.yml,\n  openapi/capepartners-fr-interest-api-openapi.yml, openapi/capepartners-fr-mandate-api-openapi.yml,\n  openapi/capepartners-fr-matching-api-openapi.yml, openapi/capepartners-fr-pairings-api-openapi.yml,\n  openapi/capepartners-fr-registration-api-openapi.yml, openapi/capepartners-fr-search-api-openapi.yml,\n  openapi/capepartners-fr-valuation-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this\
  \ API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 32\n    acting: 16\n  by_consequence:\n    read: 32\n    write: 15\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/activity/{session_id}\n  method: get\n  operationId: getApiActivityBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nda/sign\n  method: post\n  operationId: postApiNdaSign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/nda/text\n  method: get\n  operationId: getApiNdaText\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tos/text\n  method: get\n  operationId: getApiTosText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dq/enqueue\n  method: post\n  operationId: postApiDqEnqueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/deal-flow/{session_id}\n  method: get\n  operationId: getApiDealFlowBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/watchlist\n  method: post\n  operationId: postApiWatchlist\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api\n  method: get\n  operationId: getApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/llms.txt\n  method: get\n  operationId: getWellKnownLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ai-plugin.json\n  method: get\n  operationId: getWellKnownAiPluginJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /robots.txt\n  method: get\n  operationId: getRobotsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  operationId: getSitemapXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: getWellKnownAgentCardJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /a2a\n  method: post\n  operationId: postA2a\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/message:send\n  method: post\n  operationId: postA2aMessage:send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/tasks\n  method: get\n  operationId: getA2aTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/tasks/{id}\n  method: get\n\
  \  operationId: getA2aTasksById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/exchange/spec\n  method: get\n  operationId: getApiExchangeSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/exchange/manifest\n  method: post\n  operationId: postApiExchangeManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/exchange/answer/{msgid}\n  method: get\n  operationId: getApiExchangeAnswerByMsgid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/exchange/reply\n  method: post\n  operationId: postApiExchangeReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/{token}/thread\n  method: get\n  operationId: getEngageByTokenThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /engage/{token}/reply\n  method: post\n  operationId: postEngageByTokenReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/workspace/{session_id}\n\
  \  method: get\n  operationId: getApiWorkspaceBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/workspace/join\n  method: post\n  operationId: postApiWorkspaceJoin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/session/{session_id}\n  method: get\n  operationId: getApiSessionBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/session/{session_id}\n  method: post\n  operationId: postApiSessionBySessionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/infomemo/{session_id}\n  method: get\n  operationId: getApiInfomemoBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/infomemo/{session_id}/download\n  method: get\n  operationId: getApiInfomemoBySessionIdDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/light-infomemo/{session_id}/{pair_id}\n  method: get\n  operationId: getApiLightInfomemoBySessionIdByPairId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/product-analysis/{session_id}/{pairing_id}\n  method:\
  \ get\n  operationId: getApiProductAnalysisBySessionIdByPairingId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/interest-signals/{session_id}\n  method: get\n  operationId: getApiInterestSignalsBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/interest-signals/{session_id}/ack\n  method: post\n  operationId: postApiInterestSignalsBySessionIdAck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mandate/{session_id}\n  method: get\n  operationId: getApiMandateBySessionId\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mandate/{session_id}/preview\n  method: get\n  operationId: getApiMandateBySessionIdPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mandate/request\n  method: post\n  operationId: postApiMandateRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/matches/{session_id}\n  method: get\n  operationId: getApiMatchesBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/matched-names/{session_id}\n  method: get\n\
  \  operationId: getApiMatchedNamesBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/seller-name/{session_id}\n  method: get\n  operationId: getApiSellerNameBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pairings/{session_id}\n  method: get\n  operationId: getApiPairingsBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pairings/create\n  method: post\n  operationId: postApiPairingsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /api/pairings/update_phase\n  method: post\n  operationId: postApiPairingsUpdatePhase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pairings/phase-request\n  method: post\n  operationId: postApiPairingsPhaseRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/submit\n  method: post\n  operationId: postApiSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/search/{session_id}\n  method: get\n  operationId: getApiSearchBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/valuation/{session_id}\n  method: get\n  operationId: getApiValuationBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/capepartners-fr/agentic-access/capepartners-fr-agentic-access.yml
summary_line: 48 operations · 16 acting
tags:
- Mergers and Acquisitions
- Deal Flow
- Valuation
- Investment
- Financial Services
- Agents
- A2A
- France
- Technology
- Software-as-a-Service
---
