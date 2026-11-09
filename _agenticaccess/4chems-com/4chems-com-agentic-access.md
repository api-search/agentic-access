---
acting_count: 37
action_class_counts:
  acting: 37
  connected: 20
api_specs:
- filename: 4chems-com-authz-api-openapi.yml
  format: yaml
  label: 4chems Authz API
  slug: 4chems-com-authz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-authz-api-openapi.yml
- filename: 4chems-com-billing-api-openapi.yml
  format: yaml
  label: 4chems Billing API
  slug: 4chems-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-billing-api-openapi.yml
- filename: 4chems-com-catalog-api-openapi.yml
  format: yaml
  label: 4chems Catalog API
  slug: 4chems-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-catalog-api-openapi.yml
- filename: 4chems-com-consents-api-openapi.yml
  format: yaml
  label: 4chems Consents API
  slug: 4chems-com-consents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-consents-api-openapi.yml
- filename: 4chems-com-customer-api-openapi.yml
  format: yaml
  label: 4chems Customer API
  slug: 4chems-com-customer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-customer-api-openapi.yml
- filename: 4chems-com-infra-operations-api-openapi.yml
  format: yaml
  label: 4chems Infra Operations API
  slug: 4chems-com-infra-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-infra-operations-api-openapi.yml
- filename: 4chems-com-infrastructure-api-openapi.yml
  format: yaml
  label: 4chems Infrastructure API
  slug: 4chems-com-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-infrastructure-api-openapi.yml
- filename: 4chems-com-inquiries-api-openapi.yml
  format: yaml
  label: 4chems Inquiries API
  slug: 4chems-com-inquiries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-inquiries-api-openapi.yml
- filename: 4chems-com-invitations-api-openapi.yml
  format: yaml
  label: 4chems Invitations API
  slug: 4chems-com-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-invitations-api-openapi.yml
- filename: 4chems-com-onboarding-api-openapi.yml
  format: yaml
  label: 4chems Onboarding API
  slug: 4chems-com-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-onboarding-api-openapi.yml
- filename: 4chems-com-operations-api-openapi.yml
  format: yaml
  label: 4chems Operations API
  slug: 4chems-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-operations-api-openapi.yml
- filename: 4chems-com-reference-api-openapi.yml
  format: yaml
  label: 4chems Reference API
  slug: 4chems-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-reference-api-openapi.yml
- filename: 4chems-com-tenants-api-openapi.yml
  format: yaml
  label: 4chems Tenants API
  slug: 4chems-com-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-tenants-api-openapi.yml
- filename: 4chems-com-trials-api-openapi.yml
  format: yaml
  label: 4chems Trials API
  slug: 4chems-com-trials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4chems-com/openapi/4chems-com-trials-api-openapi.yml
consequence_counts:
  physical: 3
  read: 20
  safety-critical: 4
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: 4Chems Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /infra/catalog/templates/{code}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /infra/kill-switches/{name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/tenant/invitations/{invitation_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/tenant/members/{sub}/assignments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ops/notifications/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ops/notifications/email/templated
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/onboarding/access-requests/{access_request_id}:withdraw
operation_count: 57
overview: '4chems exposes 57 API operations that an AI agent could call, of which 37 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 30 write, 3 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 4chems
provider_slug: 4chems-com
slug: 4chems-com-agentic-access
source_filename: 4chems-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/4chems-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 20\n    acting: 37\n  by_consequence:\n    read: 20\n    write: 30\n    safety-critical: 4\n    physical: 3\n  human_in_the_loop_required: 4\noperations:\n- path: /v1/me/access\n  method: get\n  operationId: get_my_access\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tenant/members\n  method: get\n  operationId: list_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/tenant/members/{sub}/assignments\n  method: post\n  operationId: grant_assignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tenant/members/{sub}/assignments/{id}\n  method: delete\n  operationId: revoke_assignment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /infra/nodes\n  method: get\n  operationId: list_nodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /infra/whoami\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infra/kill-switches\n  method: get\n  operationId: list_kill_switches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infra/kill-switches/{name}\n  method: patch\n  operationId: set_kill_switch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /infra/catalog/templates\n  method: get\n  operationId: list_all_catalog_templates\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infra/catalog/templates\n  method: post\n  operationId: create_catalog_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infra/catalog/templates/{code}\n  method: patch\n  operationId: update_catalog_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infra/catalog/templates/{code}/disable\n  method: post\n  operationId: disable_catalog_template\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /infra/operations/\n  method: get\n  operationId: list_infra_operations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infra/operations/{operation_id}\n  method: get\n  operationId: get_infra_operation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infra/operations/{operation_id}/retry\n  method: post\n  operationId: retry_operation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infra/operations/{operation_id}/cancel\n  method: post\n  operationId: cancel_operation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infra/tenants\n  method: post\n  operationId: create_tenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infra/tenants\n  method: get\n  operationId: list_tenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /infra/tenants/{tenant_id}\n  method: get\n  operationId: get_tenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infra/trials\n  method: post\n  operationId: create_trial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infra/trials/{trial_id}\n  method: get\n  operationId: get_trial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infra/trials/{trial_id}\n  method: delete\n  operationId: teardown_trial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infra/trials/{trial_id}:extend\n  method: post\n  operationId: extend_trial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infra/trials/{trial_id}:load-data\n  method: post\n  operationId: load_trial_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infra/trials/{trial_id}:erase-data\n  method: post\n  operationId: erase_trial_data\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ops/notifications/email\n  method: post\n  operationId: send_email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ops/notifications/email/templated\n  method: post\n  operationId: send_templated_email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ops/operations/{operation_id}\n  method: get\n  operationId: get_operation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operations/{operation_id}\n  method: get\n  operationId: get_my_operation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tenant/billing\n  method: get\n  operationId: get_billing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tenant/billing\n  method: put\n  operationId: complete_billing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tenant/services\n  method: get\n  operationId: list_tenant_services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tenant/services\n  method: post\n  operationId: add_tenant_service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog/templates\n  method: get\n  operationId: get_catalog_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/consents\n  method: post\n  operationId: record_consent\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/consents\n  method: get\n  operationId: list_consents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reference/legal-entity-types\n  method: get\n  operationId: get_legal_entity_types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tenant/invitations\n  method: post\n  operationId: create_invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tenant/invitations\n  method: get\n  operationId: list_invitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tenant/invitations/{invitation_id}\n  method: delete\n  operationId: revoke_invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invitations/{token}/accept\n  method: post\n  operationId: accept_invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/route\n  method: get\n  operationId: get_onboarding_route\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/onboarding/access-requests\n  method: post\n  operationId: create_access_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/access-requests/{access_request_id}:approve\n  method: post\n  operationId: approve_access_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/access-requests/{access_request_id}:dismiss\n  method: post\n  operationId: dismiss_access_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/access-requests/{access_request_id}:withdraw\n  method: post\n  operationId: withdraw_access_request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/tenants\n  method: post\n  operationId:\
  \ create_self_service_tenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/entry\n  method: post\n  operationId: check_entry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/enrichment\n  method: post\n  operationId: enrich_domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/onboarding/login/device\n  method: post\n  operationId: start_device_login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/login/device/verify\n  method: post\n  operationId: verify_device_login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/registrations/device\n  method: post\n  operationId: start_registration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/registrations/device/verify\n  method: post\n  operationId: verify_registration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/registrations/account\n  method: post\n  operationId: start_account_registration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/onboarding/registrations/account/verify\n  method: post\n  operationId: verify_account_registration\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inquiries\n  method: post\n  operationId: start_inquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inquiries/verify\n  method: post\n  operationId: verify_inquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/4chems-com/agentic-access/4chems-com-agentic-access.yml
summary_line: 57 operations · 37 acting · 4 human-in-the-loop
tags:
- Chemicals
- Regulatory
- Artificial Intelligence
- Hosting
- Consulting
- EU
---
