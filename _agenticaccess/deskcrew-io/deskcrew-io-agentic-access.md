---
acting_count: 117
action_class_counts:
  acting: 117
  connected: 70
api_specs:
- filename: deskcrew-io-app-api-openapi.yml
  format: yaml
  label: DeskCrew App API
  slug: deskcrew-io-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-app-api-openapi.yml
- filename: deskcrew-io-billing-api-openapi.yml
  format: yaml
  label: DeskCrew Billing API
  slug: deskcrew-io-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-billing-api-openapi.yml
- filename: deskcrew-io-bounties-api-openapi.yml
  format: yaml
  label: DeskCrew Bounties API
  slug: deskcrew-io-bounties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-bounties-api-openapi.yml
- filename: deskcrew-io-changelog-api-openapi.yml
  format: yaml
  label: DeskCrew Changelog API
  slug: deskcrew-io-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-changelog-api-openapi.yml
- filename: deskcrew-io-changes-api-openapi.yml
  format: yaml
  label: DeskCrew Changes API
  slug: deskcrew-io-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-changes-api-openapi.yml
- filename: deskcrew-io-customers-api-openapi.yml
  format: yaml
  label: DeskCrew Customers API
  slug: deskcrew-io-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-customers-api-openapi.yml
- filename: deskcrew-io-devices-api-openapi.yml
  format: yaml
  label: DeskCrew Devices API
  slug: deskcrew-io-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-devices-api-openapi.yml
- filename: deskcrew-io-errors-api-openapi.yml
  format: yaml
  label: DeskCrew Errors API
  slug: deskcrew-io-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-errors-api-openapi.yml
- filename: deskcrew-io-issues-api-openapi.yml
  format: yaml
  label: DeskCrew Issues API
  slug: deskcrew-io-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-issues-api-openapi.yml
- filename: deskcrew-io-kb-api-openapi.yml
  format: yaml
  label: DeskCrew Kb API
  slug: deskcrew-io-kb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-kb-api-openapi.yml
- filename: deskcrew-io-me-api-openapi.yml
  format: yaml
  label: DeskCrew Me API
  slug: deskcrew-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-me-api-openapi.yml
- filename: deskcrew-io-paid-agent-tools-api-openapi.yml
  format: yaml
  label: DeskCrew Paid agent tools API
  slug: deskcrew-io-paid-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-paid-agent-tools-api-openapi.yml
- filename: deskcrew-io-tickets-api-openapi.yml
  format: yaml
  label: DeskCrew Tickets API
  slug: deskcrew-io-tickets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-tickets-api-openapi.yml
- filename: deskcrew-io-webhooks-api-openapi.yml
  format: yaml
  label: DeskCrew Webhooks API
  slug: deskcrew-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskcrew-io/openapi/deskcrew-io-webhooks-api-openapi.yml
consequence_counts:
  physical: 14
  read: 70
  safety-critical: 3
  write: 100
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Deskcrew Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/app/agents/credentials/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/app/api-keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/x402/tools/deskcrew/rotate_board_key
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/app/approvals/{id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/app/bounties
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/app/broadcasts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/app/kb/categories/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/app/nft/referral
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/app/send-domain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/app/send-domain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/app/send-domain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/bounties/deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/kb/categories/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tickets/{id}/reply
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/x402/tools/deskcrew/nft_wallet
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/x402/tools/deskcrew/subscribe_events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/x402/tools/deskcrew/wallet_check
operation_count: 187
overview: 'DeskCrew exposes 187 API operations that an AI agent could call, of which 117 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 70 read, 100 write, 14 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DeskCrew
provider_slug: deskcrew-io
slug: deskcrew-io-agentic-access
source_filename: deskcrew-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/deskcrew-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 187\n  by_action_class:\n    connected: 70\n    acting: 117\n  by_consequence:\n    read: 70\n    write: 100\n    physical: 14\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /api/v1/tickets\n  method: get\n  operationId: get_api_v1_tickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tickets\n  method: post\n  operationId: post_api_v1_tickets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tickets/{id}\n  method: get\n  operationId: get_api_v1_tickets__id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tickets/{id}/replies\n  method: post\n  operationId: post_api_v1_tickets__id__replies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tickets/{id}/reply\n  method: post\n  operationId: post_api_v1_tickets__id__reply\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/kb\n  method: get\n  operationId: get_api_v1_kb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kb\n  method: post\n  operationId: post_api_v1_kb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/kb/{id}\n  method: get\n  operationId: get_api_v1_kb__id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kb/{id}\n  method:\
  \ patch\n  operationId: patch_api_v1_kb__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/kb/{id}\n  method: delete\n  operationId: delete_api_v1_kb__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/kb/categories\n  method: get\n  operationId: get_api_v1_kb_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kb/categories\n  method: post\n  operationId: post_api_v1_kb_categories\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/kb/categories/{id}\n  method: get\n  operationId: get_api_v1_kb_categories__id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kb/categories/{id}\n  method: patch\n  operationId: patch_api_v1_kb_categories__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/kb/categories/{id}\n  method:\
  \ delete\n  operationId: delete_api_v1_kb_categories__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/issues\n  method: get\n  operationId: get_api_v1_issues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/issues\n  method: post\n  operationId: post_api_v1_issues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/issues/{id}\n  method: get\n  operationId: get_api_v1_issues__id_\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/issues/{id}\n  method: patch\n  operationId: patch_api_v1_issues__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/issues/{id}\n  method: delete\n  operationId: delete_api_v1_issues__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/changelog\n  method: get\n  operationId: get_api_v1_changelog\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/changelog\n  method: post\n  operationId: post_api_v1_changelog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/changelog/{id}\n  method: get\n  operationId: get_api_v1_changelog__id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/changelog/{id}\n  method: patch\n  operationId: patch_api_v1_changelog__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/changelog/{id}\n  method: delete\n  operationId: delete_api_v1_changelog__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers\n  method: get\n  operationId: get_api_v1_customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  operationId: get_api_v1_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/devices/me\n  method: patch\n  operationId: patch_api_v1_devices_me\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/devices/me\n  method: delete\n  operationId: delete_api_v1_devices_me\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing\n  method: get\n  operationId: get_api_v1_billing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/apple\n  method: post\n  operationId: post_api_v1_billing_apple\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/tickets\n  method: get\n  operationId: get_api_v1_app_tickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/tickets\n  method: post\n  operationId: post_api_v1_app_tickets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/tickets/search\n  method: get\n  operationId: get_api_v1_app_tickets_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/tickets/counts\n\
  \  method: post\n  operationId: post_api_v1_app_tickets_counts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/tickets/bulk\n  method: post\n  operationId: post_api_v1_app_tickets_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/tickets/{id}\n  method: get\n  operationId: get_api_v1_app_tickets__id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/tickets/{id}\n  method: patch\n\
  \  operationId: patch_api_v1_app_tickets__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/tickets/{id}/reply\n  method: post\n  operationId: post_api_v1_app_tickets__id__reply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/tickets/{id}/reopen\n  method: post\n  operationId: post_api_v1_app_tickets__id__reopen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/tickets/{id}/request-contact\n  method: post\n  operationId: post_api_v1_app_tickets__id__request-contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/tickets/{id}/assignable\n  method: get\n  operationId: get_api_v1_app_tickets__id__assignable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/replies/{id}/retract\n  method: post\n  operationId: post_api_v1_app_replies__id__retract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/approvals/pending\n  method: get\n  operationId: get_api_v1_app_approvals_pending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/approvals/{id}/approve\n  method: post\n  operationId: post_api_v1_app_approvals__id__approve\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/approvals/{id}/reject\n  method: post\n  operationId: post_api_v1_app_approvals__id__reject\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/approvals/{id}/edit\n  method: post\n  operationId: post_api_v1_app_approvals__id__edit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/approvals/{id}/reason\n  method: post\n  operationId: post_api_v1_app_approvals__id__reason\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/overview\n\
  \  method: get\n  operationId: get_api_v1_app_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/notifications\n  method: get\n  operationId: get_api_v1_app_notifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/notifications\n  method: patch\n  operationId: patch_api_v1_app_notifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/reports\n  method: get\n  operationId: get_api_v1_app_reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/reports/timezone\n  method: patch\n  operationId: patch_api_v1_app_reports_timezone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/reports/{id}\n  method: get\n  operationId: get_api_v1_app_reports__id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/account\n  method: get\n  operationId: get_api_v1_app_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/account\n  method: patch\n  operationId: patch_api_v1_app_account\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/kb/articles\n  method: get\n  operationId: get_api_v1_app_kb_articles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/kb/articles\n  method: post\n  operationId: post_api_v1_app_kb_articles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/kb/articles/{id}\n  method: get\n  operationId: get_api_v1_app_kb_articles__id_\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/kb/articles/{id}\n  method: patch\n  operationId: patch_api_v1_app_kb_articles__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/kb/articles/{id}\n  method: delete\n  operationId: delete_api_v1_app_kb_articles__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/kb/categories\n  method: get\n  operationId: get_api_v1_app_kb_categories\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/kb/categories\n  method: post\n  operationId: post_api_v1_app_kb_categories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/kb/categories/{id}\n  method: patch\n  operationId: patch_api_v1_app_kb_categories__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/kb/categories/{id}\n  method: delete\n  operationId: delete_api_v1_app_kb_categories__id_\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/team\n  method: get\n  operationId: get_api_v1_app_team\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/team\n  method: post\n  operationId: post_api_v1_app_team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/team/{id}\n  method: patch\n  operationId: patch_api_v1_app_team__id_\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/team/{id}\n  method: delete\n  operationId: delete_api_v1_app_team__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/team/devices\n  method: get\n  operationId: get_api_v1_app_team_devices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/team/devices/{id}\n  method: delete\n  operationId: delete_api_v1_app_team_devices__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/api-keys\n  method: get\n  operationId: get_api_v1_app_api-keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/api-keys\n  method: post\n  operationId: post_api_v1_app_api-keys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/api-keys/{id}\n  method: post\n  operationId: post_api_v1_app_api-keys__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/api-keys/{id}\n  method: delete\n  operationId: delete_api_v1_app_api-keys__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/app/agents/door\n  method: get\n  operationId: get_api_v1_app_agents_door\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/agents/door\n  method: patch\n  operationId: patch_api_v1_app_agents_door\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/agents/credentials\n  method: get\n  operationId: get_api_v1_app_agents_credentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/agents/credentials\n  method: post\n  operationId: post_api_v1_app_agents_credentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/agents/credentials/{id}\n  method: patch\n  operationId: patch_api_v1_app_agents_credentials__id_\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/agents/credentials/{id}\n  method: delete\n  operationId: delete_api_v1_app_agents_credentials__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/app/agents/external\n  method: get\n  operationId: get_api_v1_app_agents_external\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/agents/external\n  method: patch\n  operationId: patch_api_v1_app_agents_external\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/install\n  method: get\n  operationId: get_api_v1_app_install\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/install\n  method: patch\n  operationId: patch_api_v1_app_install\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/install/origins\n  method: post\n  operationId: post_api_v1_app_install_origins\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/install/origins\n  method: delete\n  operationId: delete_api_v1_app_install_origins\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/install/rotate\n  method: post\n  operationId: post_api_v1_app_install_rotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /api/v1/app/install/identify-secret\n  method: get\n  operationId: get_api_v1_app_install_identify-secret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/branding\n  method: get\n  operationId: get_api_v1_app_branding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/branding\n  method: patch\n  operationId: patch_api_v1_app_branding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/branding/logo\n  method: post\n  operationId: post_api_v1_app_branding_logo\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/branding/logo\n  method: delete\n  operationId: delete_api_v1_app_branding_logo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/domains\n  method: get\n  operationId: get_api_v1_app_domains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/domains\n  method: post\n  operationId: post_api_v1_app_domains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/domains\n  method: delete\n  operationId: delete_api_v1_app_domains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/send-domain\n  method: get\n  operationId: get_api_v1_app_send-domain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/send-domain\n  method: post\n  operationId: post_api_v1_app_send-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/send-domain\n  method: patch\n  operationId: patch_api_v1_app_send-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/send-domain\n  method: delete\n  operationId: delete_api_v1_app_send-domain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/inbox-forwarding\n  method: get\n  operationId: get_api_v1_app_inbox-forwarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/inbox-forwarding\n  method: patch\n  operationId: patch_api_v1_app_inbox-forwarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/collections\n  method: get\n  operationId: get_api_v1_app_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (57 KB total) ---\n# Full source:\
  \ https://artifacts.apis.io/deskcrew-io/agentic-access/deskcrew-io-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/deskcrew-io/agentic-access/deskcrew-io-agentic-access.yml
summary_line: 187 operations · 117 acting · 3 human-in-the-loop
tags:
- Company
- Help Desk
- AI Agents
- MCP
- Support
---
