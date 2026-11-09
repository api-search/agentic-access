---
acting_count: 41
action_class_counts:
  acting: 41
  connected: 23
api_specs:
- filename: coldrig-dev-account-api-openapi.yml
  format: yaml
  label: Coldrig Account API
  slug: coldrig-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-account-api-openapi.yml
- filename: coldrig-dev-bootstrap-api-openapi.yml
  format: yaml
  label: Coldrig Bootstrap API
  slug: coldrig-dev-bootstrap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-bootstrap-api-openapi.yml
- filename: coldrig-dev-byo-domains-api-openapi.yml
  format: yaml
  label: Coldrig Byo Domains API
  slug: coldrig-dev-byo-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-byo-domains-api-openapi.yml
- filename: coldrig-dev-campaigns-api-openapi.yml
  format: yaml
  label: Coldrig Campaigns API
  slug: coldrig-dev-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-campaigns-api-openapi.yml
- filename: coldrig-dev-compliance-api-openapi.yml
  format: yaml
  label: Coldrig Compliance API
  slug: coldrig-dev-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-compliance-api-openapi.yml
- filename: coldrig-dev-dashboard-api-openapi.yml
  format: yaml
  label: Coldrig Dashboard API
  slug: coldrig-dev-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-dashboard-api-openapi.yml
- filename: coldrig-dev-inbox-api-openapi.yml
  format: yaml
  label: Coldrig Inbox API
  slug: coldrig-dev-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-inbox-api-openapi.yml
- filename: coldrig-dev-infrastructure-api-openapi.yml
  format: yaml
  label: Coldrig Infrastructure API
  slug: coldrig-dev-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-infrastructure-api-openapi.yml
- filename: coldrig-dev-leads-api-openapi.yml
  format: yaml
  label: Coldrig Leads API
  slug: coldrig-dev-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-leads-api-openapi.yml
- filename: coldrig-dev-messages-api-openapi.yml
  format: yaml
  label: Coldrig Messages API
  slug: coldrig-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-messages-api-openapi.yml
- filename: coldrig-dev-sandbox-api-openapi.yml
  format: yaml
  label: Coldrig Sandbox API
  slug: coldrig-dev-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-sandbox-api-openapi.yml
- filename: coldrig-dev-webhooks-api-openapi.yml
  format: yaml
  label: Coldrig Webhooks API
  slug: coldrig-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-webhooks-api-openapi.yml
consequence_counts:
  physical: 3
  read: 23
  safety-critical: 3
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Coldrig Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /campaigns/{id}/pause
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dashboard/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /experiments/{id}/retire
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /threads/{id}/reply
operation_count: 64
overview: 'Coldrig exposes 64 API operations that an AI agent could call, of which 41 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 35 write, 3 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Coldrig
provider_slug: coldrig-dev
slug: coldrig-dev-agentic-access
source_filename: coldrig-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/coldrig-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 64\n  by_action_class:\n    acting: 41\n    connected: 23\n  by_consequence:\n    write: 35\n    physical: 3\n    read: 23\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /signup\n  method: post\n  operationId: signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout\n  method: post\n  operationId: create_checkout_link\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setup-infrastructure\n  method: post\n  operationId: setup_infrastructure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infrastructure-status\n  method: get\n  operationId: infrastructure_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /remove-mailboxes\n  method: post\n  operationId: remove_mailboxes\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancel\n  method: post\n  operationId: cancel_subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/portal\n  method: post\n  operationId: billing_portal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/invoices\n  method: get\n  operationId:\
  \ billing_invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: post\n  operationId: launch_campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns\n  method: get\n  operationId: list_campaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/results\n  method: get\n  operationId: campaign_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/experiments\n  method: post\n\
  \  operationId: experiment_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/experiments\n  method: get\n  operationId: experiment_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experiments/{id}/retire\n  method: post\n  operationId: experiment_retire\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /experiments/{id}/conclude\n  method: post\n  operationId:\
  \ experiment_conclude\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/breakdown\n  method: get\n  operationId: experiment_breakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experiments/patterns\n  method: get\n  operationId: experiment_patterns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experiments/sharing\n  method: get\n  operationId: experiment_sharing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experiments/sharing\n\
  \  method: put\n  operationId: experiment_set_sharing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/leads\n  method: post\n  operationId: add_leads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/pause\n  method: post\n  operationId: pause\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /campaigns/{id}/resume\n  method: post\n  operationId: resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/pause-all\n  method: post\n  operationId: pause_all\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/plan\n  method: post\n  operationId: plan_campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /demo/run\n  method: post\n  operationId: demo_run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics\n  method: get\n  operationId: metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbox\n  method: get\n  operationId: inbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /threads/{id}\n  method: get\n  operationId: thread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /threads/{id}/reply\n  method: post\n  operationId: reply\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threads/{id}/mark\n  method: post\n  operationId: mark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threads/{id}/label\n  method: post\n  operationId: label_thread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activity\n  method: get\n  operationId: activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/session\n  method: post\n  operationId: dashboard_login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/logout\n  method: post\n  operationId: dashboard_logout\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dashboard/views\n  method: get\n  operationId: get_dashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/views\n  method: post\n  operationId: configure_dashboard_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/views/{id}\n  method: get\n  operationId: get_dashboard_view\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/views/{id}\n  method: put\n  operationId: configure_dashboard_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/views/{id}\n  method: delete\n  operationId: configure_dashboard_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/views/{id}/default\n  method: post\n  operationId: configure_dashboard_promote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions\n  method: get\n  operationId: get_webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-subscriptions\n  method: post\n  operationId: configure_webhook_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions/{id}\n  method: get\n  operationId: get_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /webhook-subscriptions/{id}\n  method: put\n  operationId: configure_webhook_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions/{id}\n  method: delete\n  operationId: configure_webhook_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connected-apps\n  method: get\n  operationId: get_connected_apps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connected-apps/{id}\n  method:\
  \ delete\n  operationId: disconnect_app\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /byo-domains\n  method: get\n  operationId: get_byo_domains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /byo-domains\n  method: post\n  operationId: register_byo_domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /byo-domains/{id}\n  method: get\n  operationId: get_byo_domain\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /byo-domains/{id}/poll-dns\n  method: post\n  operationId: poll_byo_domain_dns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /byo-domains/{id}/consent\n  method: post\n  operationId: acknowledge_byo_consent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /byo-domains/{id}/managed-mailboxes\n  method: post\n  operationId: request_managed_byo_mailboxes\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /byo-domains/{id}/connect-mailbox\n  method: post\n  operationId: connect_byo_mailbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads\n  method: get\n  operationId: list_leads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/suppress\n  method: post\n  operationId: suppress_lead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads/disposition\n  method: post\n  operationId: update_lead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  operationId: list_messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{id}/ack\n  method: post\n  operationId: ack_message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /messages/contact-operator\n  method: post\n  operationId: contact_operator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/feedback\n  method: post\n  operationId: submit_feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unsubscribe\n  method: get\n  operationId: unsubscribe_confirm_page\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /unsubscribe\n  method: post\n  operationId: unsubscribe_confirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/coldrig-dev/agentic-access/coldrig-dev-agentic-access.yml
summary_line: 64 operations · 41 acting · 3 human-in-the-loop
tags:
- Cold Email
- Outreach
- AI Agents
- Email Infrastructure
---
