---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 8
api_specs:
- filename: sendsonar-com-accounts-api-openapi.yml
  format: yaml
  label: Sonar Accounts API
  slug: sendsonar-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-accounts-api-openapi.yml
- filename: sendsonar-com-campaigns-api-openapi.yml
  format: yaml
  label: Sonar Campaigns API
  slug: sendsonar-com-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-campaigns-api-openapi.yml
- filename: sendsonar-com-conversations-api-openapi.yml
  format: yaml
  label: Sonar Conversations API
  slug: sendsonar-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-conversations-api-openapi.yml
- filename: sendsonar-com-customers-api-openapi.yml
  format: yaml
  label: Sonar Customers API
  slug: sendsonar-com-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-customers-api-openapi.yml
- filename: sendsonar-com-events-api-openapi.yml
  format: yaml
  label: Sonar Events API
  slug: sendsonar-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-events-api-openapi.yml
- filename: sendsonar-com-messages-api-openapi.yml
  format: yaml
  label: Sonar Messages API
  slug: sendsonar-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-messages-api-openapi.yml
- filename: sendsonar-com-phone-numbers-api-openapi.yml
  format: yaml
  label: Sonar Phone Numbers API
  slug: sendsonar-com-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-phone-numbers-api-openapi.yml
- filename: sendsonar-com-roles-api-openapi.yml
  format: yaml
  label: Sonar Roles API
  slug: sendsonar-com-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-roles-api-openapi.yml
- filename: sendsonar-com-users-api-openapi.yml
  format: yaml
  label: Sonar Users API
  slug: sendsonar-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-users-api-openapi.yml
- filename: sendsonar-com-webhooks-api-openapi.yml
  format: yaml
  label: Sonar Webhooks API
  slug: sendsonar-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendsonar-com/openapi/sendsonar-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 3
  read: 8
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sendsonar Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/campaigns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/campaigns/send_personalized_campaign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages
operation_count: 27
overview: 'Sonar exposes 27 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 16 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sonar
provider_slug: sendsonar-com
slug: sendsonar-com-agentic-access
source_filename: sendsonar-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: generated\nsource: openapi/sendsonar-com-api-settings-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 19\n    connected: 8\n  by_consequence:\n    write: 16\n    physical: 3\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/accounts\n  method: post\n  operationId: create-new-sonar-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns\n  method: post\n  operationId: send-campaign\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns/send_personalized_campaign\n  method: post\n  operationId: personalized-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conversations/{id}\n  method: get\n  operationId: get-conversation-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n\
  \  method: get\n  operationId: get-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: post\n  operationId: addupdate-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/close\n  method: post\n  operationId: close-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/follow_ups\n  method: post\n  operationId: follow-up-endpoint\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/follow_ups\n  method: delete\n  operationId: remove-follow-up\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/personal_data?token=company_private_token&phone_number=contact_phone_number\n  method: get\n  operationId: gdpr-get-request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/personal_data?token=your_private_token&phone_number=contact_phone_number\n\
  \  method: delete\n  operationId: gdpr-delete-request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/properties\n  method: delete\n  operationId: delete-customer-properties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/unassign\n  method: post\n  operationId: unassign-agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events\n  method: post\n  operationId: events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: post\n  operationId: send-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/doi_prompts\n  method: post\n  operationId: double-opt-in-prompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{external_message_id}/tags\n  method: post\n  operationId: append-tag-to-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/phone_numbers/available\n  method: get\n  operationId: available-phone-number\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/roles\n  method: get\n  operationId: get-account-roles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/roles\n  method: post\n  operationId: create-new-role-permission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users\n  method: get\n  operationId: get-all-users-from-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: post\n  operationId: invite-new-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{:id}\n  method: get\n  operationId: get-specific-user-by-id\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: get\n  operationId: get-webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: create-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/:id\n  method: put\n  operationId: update-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/webhooks/:id\n  method: delete\n  operationId: delete-webhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/sendsonar-com/agentic-access/sendsonar-com-agentic-access.yml
summary_line: 27 operations · 19 acting
tags:
- Company
- SMS
- Messaging
- Sales
- Automation
---
