---
acting_count: 41
action_class_counts:
  acting: 41
  connected: 43
api_specs:
- filename: plainrouter-actiondryrunapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Dry Run API
  slug: plainrouter-actiondryrunapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-actiondryrunapi-api-openapi.yml
- filename: plainrouter-actionproposalapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Proposal API
  slug: plainrouter-actionproposalapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-actionproposalapi-api-openapi.yml
- filename: plainrouter-actionreadapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Read API
  slug: plainrouter-actionreadapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-actionreadapi-api-openapi.yml
- filename: plainrouter-actionruleapi-api-openapi.yml
  format: yaml
  label: Plainrouter Action Rule API
  slug: plainrouter-actionruleapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-actionruleapi-api-openapi.yml
- filename: plainrouter-adtestapi-api-openapi.yml
  format: yaml
  label: Plainrouter Ad Test API
  slug: plainrouter-adtestapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-adtestapi-api-openapi.yml
- filename: plainrouter-agentcontext-api-openapi.yml
  format: yaml
  label: Plainrouter Agent Context API
  slug: plainrouter-agentcontext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-agentcontext-api-openapi.yml
- filename: plainrouter-cookiedeclaration-api-openapi.yml
  format: yaml
  label: Plainrouter Cookie Declaration API
  slug: plainrouter-cookiedeclaration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-cookiedeclaration-api-openapi.yml
- filename: plainrouter-creative-api-openapi.yml
  format: yaml
  label: Plainrouter Creative API
  slug: plainrouter-creative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-creative-api-openapi.yml
- filename: plainrouter-deploymentplan-api-openapi.yml
  format: yaml
  label: Plainrouter Deployment Plan API
  slug: plainrouter-deploymentplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-deploymentplan-api-openapi.yml
- filename: plainrouter-draftbatchfileimport-api-openapi.yml
  format: yaml
  label: Plainrouter Draft Batch File Import API
  slug: plainrouter-draftbatchfileimport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-draftbatchfileimport-api-openapi.yml
- filename: plainrouter-event-api-openapi.yml
  format: yaml
  label: Plainrouter Event API
  slug: plainrouter-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-event-api-openapi.yml
- filename: plainrouter-launchpolicy-api-openapi.yml
  format: yaml
  label: Plainrouter Launch Policy API
  slug: plainrouter-launchpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-launchpolicy-api-openapi.yml
- filename: plainrouter-metainventoryexposure-api-openapi.yml
  format: yaml
  label: Plainrouter Meta Inventory Exposure API
  slug: plainrouter-metainventoryexposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-metainventoryexposure-api-openapi.yml
- filename: plainrouter-operations-api-openapi.yml
  format: yaml
  label: Plainrouter Operations API
  slug: plainrouter-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-operations-api-openapi.yml
- filename: plainrouter-sandbox-api-openapi.yml
  format: yaml
  label: Plainrouter Sandbox API
  slug: plainrouter-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/openapi/plainrouter-sandbox-api-openapi.yml
consequence_counts:
  physical: 7
  read: 43
  safety-critical: 2
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Plainrouter Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /destinations/{destination}/test-purchase
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /destinations/{destination}/test-purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspace}/admin/plans
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /workspaces/{workspace}/admin/plans/{deployment_plan}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspace}/admin/plans/{deployment_plan}/copy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspace}/admin/plans/{deployment_plan}/copy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspace}/admin/plans/{deployment_plan}/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspace}/admin/plans/{deployment_plan}/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspace}/admin/plans/{deployment_plan}/validate
operation_count: 84
overview: 'Plainrouter exposes 84 API operations that an AI agent could call, of which 41 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 43 read, 32 write, 7 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Plainrouter
provider_slug: plainrouter
slug: plainrouter-agentic-access
source_filename: plainrouter-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/dev-plainrouter-openapi.json, openapi/plainrouter-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 84\n  by_action_class:\n    acting: 41\n    connected: 43\n  by_consequence:\n    write: 32\n    read: 43\n    physical: 7\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /agent/workspaces/{workspace}/actions/dry-run\n  method: post\n  operationId: actions.api.dry-run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /agent/workspaces/{workspace}/actions\n  method: post\n  operationId: actions.api.propose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/workspaces/{workspace}/actions\n  method: get\n  operationId: actions.api.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/actions/policy\n  method: get\n  operationId: actions.api.policy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/actions/{action}/decision-receipt\n  method: get\n  operationId: actions.api.decision-receipt\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/actions/{action}\n  method: get\n  operationId: actions.api.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/action-batches/{actionBatch}\n  method: get\n  operationId: actions.api.batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/tests\n  method: get\n  operationId: actions.tests.api.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/tests\n  method: post\n  operationId: actions.tests.api.store\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/workspaces/{workspace}/tests/{ad_test}\n  method: get\n  operationId: actions.tests.api.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cookie-declarations/{publishableKey}\n  method: get\n  operationId: getCookieDeclaration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/creatives\n  method: post\n  operationId: storeCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/creatives/from-url\n  method: post\n  operationId: storeCreativeFromUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/plans/{deployment_plan}/copy\n  method: post\n  operationId: launch.plans.copy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/plans/{deployment_plan}/execute\n\
  \  method: post\n  operationId: launch.plans.execute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/plans\n  method: get\n  operationId: launch.plans.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/plans/{deployment_plan}\n  method: get\n  operationId: launch.plans.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: post\n  operationId: createEvent\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verification-events\n  method: post\n  operationId: verifySignalIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/ad-accounts/{account_id}/inventory/metrics\n  method: get\n  operationId: get_inventory_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/events/cursor\n  method: get\n  operationId: listEventsByCursor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations/{destination}/test-mode\n  method: patch\n  operationId: setDestinationTestMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /destinations/{destination}/test-purchase\n  method: post\n  operationId: sendTestPurchase\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /deliveries/replay\n  method: post\n  operationId: replayDeliveries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/reconciliation\n  method: get\n  operationId: getReconciliationReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/emq\n  method: get\n  operationId: getEmqReport\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-data\n  method: delete\n  operationId: deleteUserData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox\n  method: get\n  operationId: getSandbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sandbox/keys\n  method: get\n  operationId: getSandboxKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sandbox/keys\n  method: post\n  operationId: createSandboxKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/events\n  method: post\n  operationId: validateSandboxEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/keyed-events\n  method: post\n  operationId: validateSandboxEventWithKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/workspaces/{workspace}/actions/dry-run\n  method: post\n\
  \  operationId: actions.api.dry-run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/workspaces/{workspace}/actions\n  method: post\n  operationId: actions.api.propose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/workspaces/{workspace}/actions\n  method: get\n  operationId: actions.api.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/actions/policy\n  method: get\n\
  \  operationId: actions.api.policy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/actions/{action}/decision-receipt\n  method: get\n  operationId: actions.api.decision-receipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/actions/{action}\n  method: get\n  operationId: actions.api.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/action-batches/{actionBatch}\n  method: get\n  operationId: actions.api.batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/action-rules\n\
  \  method: get\n  operationId: actions.rules.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/action-rules\n  method: post\n  operationId: actions.rules.store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/workspaces/{workspace}/action-rules/{action_rule}\n  method: get\n  operationId: actions.rules.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/action-rules/{action_rule}\n  method: patch\n  operationId: actions.rules.update\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/workspaces/{workspace}/tests\n  method: get\n  operationId: actions.tests.api.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/workspaces/{workspace}/tests\n  method: post\n  operationId: actions.tests.api.store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/workspaces/{workspace}/tests/{ad_test}\n  method: get\n  operationId: actions.tests.api.show\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/context\n  method: get\n  operationId: agent.context\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - mcp:use\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cookie-declarations/{publishableKey}\n  method: get\n  operationId: getCookieDeclaration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/creatives\n  method: post\n  operationId: storeCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/creatives\n\
  \  method: get\n  operationId: launch.creatives.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/creatives/from-url\n  method: post\n  operationId: storeCreativeFromUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/creatives/{creative}/status\n  method: patch\n  operationId: launch.creatives.status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/creatives/{creative}\n\
  \  method: get\n  operationId: launch.creatives.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/plans\n  method: post\n  operationId: launch.plans.store\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/plans\n  method: get\n  operationId: launch.plans.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/plans/{deployment_plan}\n  method: patch\n  operationId: launch.plans.update\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/plans/{deployment_plan}\n  method: get\n  operationId: launch.plans.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/plans/{deployment_plan}/copy\n  method: post\n  operationId: launch.plans.copy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /workspaces/{workspace}/admin/plans/{deployment_plan}/validate\n  method: post\n  operationId: launch.plans.validate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/plans/{deployment_plan}/execute\n  method: post\n  operationId: launch.plans.execute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/launcher/import\n  method: post\n  operationId: launcher.file-import\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: post\n  operationId: createEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verification-events\n  method: post\n  operationId: verifySignalIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event}\n\
  \  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/policies\n  method: post\n  operationId: launch.policies.store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/policies\n  method: get\n  operationId: launch.policies.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/policies/{launch_policy}/retire\n  method: post\n  operationId: launch.policies.retire\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/admin/ad-accounts/{account_id}/inventory\n  method: get\n  operationId: get_account_inventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/admin/ad-accounts/{account_id}/inventory/metrics\n  method: get\n  operationId: get_inventory_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/events/cursor\n\
  \  method: get\n  operationId: listEventsByCursor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations/{destination}/test-mode\n  method: patch\n  operationId: setDestinationTestMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /destinations/{destination}/test-purchase\n  method: post\n  operationId: sendTestPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /deliveries/replay\n\
  \  method: post\n  operationId: replayDeliveries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/reconciliation\n  method: get\n  operationId: getReconciliationReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/emq\n  method: get\n  operationId: getEmqReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-data\n  method: delete\n  operationId: deleteUserData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox\n  method: get\n  operationId: getSandbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sandbox/keys\n  method: get\n  operationId: getSandboxKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sandbox/keys\n  method: post\n  operationId: createSandboxKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/events\n  method: post\n  operationId: validateSandboxEvent\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/keyed-events\n  method: post\n  operationId: validateSandboxEventWithKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plainrouter/refs/heads/main/agentic-access/plainrouter-agentic-access.yml
summary_line: 84 operations · 41 acting · 2 human-in-the-loop
tags:
- Company
- Advertising
- Developer Tools
- PaidAds
---
