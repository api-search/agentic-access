---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 19
api_specs:
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Auth API
  slug: hathora-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Apps API
  slug: hathora-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Builds API
  slug: hathora-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Deployments API
  slug: hathora-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Processes API
  slug: hathora-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Rooms API
  slug: hathora-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Discovery API
  slug: hathora-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Logs API
  slug: hathora-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Metrics API
  slug: hathora-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Billing API
  slug: hathora-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Tokens API
  slug: hathora-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
consequence_counts:
  physical: 1
  read: 19
  safety-critical: 2
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Hathora Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /processes/v3/{appId}/stop/{processId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /tokens/v1/{orgId}/revoke/{orgTokenId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/v3/{appId}/create/{buildId}
operation_count: 36
overview: 'Hathora exposes 36 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 14 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hathora
provider_slug: hathora
slug: hathora-agentic-access
source_filename: hathora-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hathora-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 17\n    connected: 19\n  by_consequence:\n    write: 14\n    read: 19\n    physical: 1\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /auth/v1/{appId}/login/anonymous\n  method: post\n  operationId: LoginAnonymous\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v1/{appId}/login/nickname\n  method: post\n  operationId:\
  \ LoginNickname\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v1/{appId}/login/google\n  method: post\n  operationId: LoginGoogle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/v2/list\n  method: get\n  operationId: GetApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/v2/create\n  method: post\n  operationId: CreateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/v2/update/{appId}\n  method: post\n  operationId: UpdateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/v2/info/{appId}\n  method: get\n  operationId: GetApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/v2/delete/{appId}\n  method: delete\n  operationId: DeleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /builds/v3/{appId}/list\n  method: get\n  operationId: GetBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /builds/v3/{appId}/create\n  method: post\n  operationId: CreateBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /builds/v3/{appId}/run/{buildId}\n  method: post\n  operationId: RunBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /builds/v3/{appId}/info/{buildId}\n  method: get\n  operationId: GetBuild\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /builds/v3/{appId}/delete/{buildId}\n  method: delete\n  operationId: DeleteBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/v3/{appId}/list\n  method: get\n  operationId: GetDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/v3/{appId}/create/{buildId}\n  method: post\n  operationId: CreateDeployment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/v3/{appId}/latest\n  method: get\n  operationId: GetLatestDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/v3/{appId}/info/{deploymentId}\n  method: get\n  operationId: GetDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes/v3/{appId}/list/latest\n  method: get\n  operationId: GetLatestProcesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /processes/v3/{appId}/create\n  method: post\n  operationId: CreateProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /processes/v3/{appId}/info/{processId}\n  method: get\n  operationId: GetProcess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes/v3/{appId}/stop/{processId}\n  method: post\n  operationId: StopProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /rooms/v2/{appId}/create\n  method: post\n  operationId: CreateRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/v2/{appId}/info/{roomId}\n  method: get\n  operationId: GetRoomInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/v2/{appId}/connectioninfo/{roomId}\n  method: get\n  operationId: GetConnectionInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/v2/{appId}/destroy/{roomId}\n  method: post\n  operationId: DestroyRoom\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery/v2/ping\n  method: get\n  operationId: GetPingServiceEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs/v1/{appId}/process/{processId}\n  method: get\n  operationId: GetLogsForProcess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs/v1/{appId}/process/{processId}/download\n  method: get\n  operationId: DownloadLogForProcess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v1/{appId}/process/{processId}\n\
  \  method: get\n  operationId: GetMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/v1/balance\n  method: get\n  operationId: GetBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/v1/invoices\n  method: get\n  operationId: GetInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/v1/paymentmethod\n  method: get\n  operationId: GetPaymentMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/v1/customerportalurl\n  method: post\n  operationId: InitStripeCustomerPortalUrl\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/v1/{orgId}/list\n  method: get\n  operationId: GetOrgTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/v1/{orgId}/create\n  method: post\n  operationId: CreateOrgToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/v1/{orgId}/revoke/{orgTokenId}\n  method: put\n  operationId: RevokeOrgToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/agentic-access/hathora-agentic-access.yml
summary_line: 36 operations · 17 acting · 2 human-in-the-loop
tags:
- Game Servers
- Multiplayer
- Compute
- Hosting
- Orchestration
---
