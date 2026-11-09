---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 19
api_specs:
- filename: audivo-dev-account-api-openapi.yml
  format: yaml
  label: audivo-dev Account API
  slug: audivo-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-account-api-openapi.yml
- filename: audivo-dev-api-keys-api-openapi.yml
  format: yaml
  label: audivo-dev API Keys API
  slug: audivo-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-api-keys-api-openapi.yml
- filename: audivo-dev-billing-api-openapi.yml
  format: yaml
  label: audivo-dev Billing API
  slug: audivo-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-billing-api-openapi.yml
- filename: audivo-dev-catalog-api-openapi.yml
  format: yaml
  label: audivo-dev Catalog API
  slug: audivo-dev-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-catalog-api-openapi.yml
- filename: audivo-dev-connected-apps-api-openapi.yml
  format: yaml
  label: audivo-dev Connected Apps API
  slug: audivo-dev-connected-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-connected-apps-api-openapi.yml
- filename: audivo-dev-data-api-openapi.yml
  format: yaml
  label: audivo-dev Data API
  slug: audivo-dev-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-data-api-openapi.yml
- filename: audivo-dev-groups-api-openapi.yml
  format: yaml
  label: audivo-dev Groups API
  slug: audivo-dev-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-groups-api-openapi.yml
- filename: audivo-dev-quotes-api-openapi.yml
  format: yaml
  label: audivo-dev Quotes API
  slug: audivo-dev-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-quotes-api-openapi.yml
- filename: audivo-dev-session-api-openapi.yml
  format: yaml
  label: audivo-dev Session API
  slug: audivo-dev-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-session-api-openapi.yml
- filename: audivo-dev-transcripts-api-openapi.yml
  format: yaml
  label: audivo-dev Transcripts API
  slug: audivo-dev-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-transcripts-api-openapi.yml
- filename: audivo-dev-uploads-api-openapi.yml
  format: yaml
  label: audivo-dev Uploads API
  slug: audivo-dev-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-uploads-api-openapi.yml
consequence_counts:
  physical: 3
  read: 19
  safety-critical: 2
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Audivo Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/connected-apps/{grant_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/billing/auto-recharge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/refund
operation_count: 36
overview: 'audivo-dev exposes 36 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 12 write, 3 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: audivo-dev
provider_slug: audivo-dev
slug: audivo-dev-agentic-access
source_filename: audivo-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/audivo-dev-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 17\n    connected: 19\n  by_consequence:\n    write: 12\n    read: 19\n    safety-critical: 2\n    physical: 3\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/transcripts\n  method: post\n  operationId: createTranscript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transcripts/{job_id}\n  method: get\n  operationId: getTranscriptJob\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/episodes/{episode_id}/transcript\n  method: get\n  operationId: getEpisodeTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reads/{read_id}\n  method: get\n  operationId: getTranscriptRead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search/shows\n  method: get\n  operationId: searchShows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/charts\n  method: get\n  operationId: getChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/quotes\n  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quotes/{quote_id}/confirm\n  method: post\n  operationId: confirmQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/groups/{group_id}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/groups/{group_id}/cancel\n  method: post\n  operationId: cancelGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shows/{show_id}/episodes\n  method: get\n  operationId: listShowEpisodes\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resolve\n  method: get\n  operationId: resolvePointer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/limits\n  method: get\n  operationId: getLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/languages\n  method: get\n  operationId: listLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/session\n  method: post\n  operationId: establishSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys/{key_id}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/oauth/requests/{request_id}\n  method: get\n  operationId: getOAuthRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oauth/requests/{request_id}/decision\n  method: post\n  operationId: decideOAuthRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connected-apps\n  method: get\n  operationId: listConnectedApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connected-apps/{grant_id}\n  method: delete\n  operationId: revokeConnectedApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/logs\n  method: get\n  operationId: listRequestLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout\n  method: post\n  operationId: createCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: createPortalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/address\n  method: get\n  operationId: getBillingAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/address\n  method: put\n  operationId: updateBillingAddress\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/auto-recharge\n  method: get\n  operationId: getAutoRecharge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/auto-recharge\n  method: put\n  operationId: updateAutoRecharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/refund\n  method: post\n  operationId: requestRefund\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/export\n  method: post\n  operationId: exportAccountData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data\n  method: delete\n  operationId: deleteAccountData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/audivo-dev/agentic-access/audivo-dev-agentic-access.yml
summary_line: 36 operations · 17 acting · 2 human-in-the-loop
tags:
- Company
- Podcasts
- Transcripts
- Audio
---
