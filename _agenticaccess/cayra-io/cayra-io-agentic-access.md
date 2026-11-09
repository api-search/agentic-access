---
acting_count: 50
action_class_counts:
  acting: 50
  connected: 45
api_specs:
- filename: cayra-io-admin-api-openapi.yml
  format: yaml
  label: Cayra Admin API
  slug: cayra-io-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-admin-api-openapi.yml
- filename: cayra-io-admin-vm-pool-api-openapi.yml
  format: yaml
  label: Cayra Admin Vm Pool API
  slug: cayra-io-admin-vm-pool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-admin-vm-pool-api-openapi.yml
- filename: cayra-io-agreements-api-openapi.yml
  format: yaml
  label: Cayra Agreements API
  slug: cayra-io-agreements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-agreements-api-openapi.yml
- filename: cayra-io-billing-api-openapi.yml
  format: yaml
  label: Cayra Billing API
  slug: cayra-io-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-billing-api-openapi.yml
- filename: cayra-io-cayra-license-server-api-openapi.yml
  format: yaml
  label: Cayra Cayra License Server API
  slug: cayra-io-cayra-license-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-cayra-license-server-api-openapi.yml
- filename: cayra-io-client-api-openapi.yml
  format: yaml
  label: Cayra Client API
  slug: cayra-io-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-client-api-openapi.yml
- filename: cayra-io-deployments-api-openapi.yml
  format: yaml
  label: Cayra Deployments API
  slug: cayra-io-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-deployments-api-openapi.yml
- filename: cayra-io-health-api-openapi.yml
  format: yaml
  label: Cayra Health API
  slug: cayra-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-health-api-openapi.yml
- filename: cayra-io-messaging-api-openapi.yml
  format: yaml
  label: Cayra Messaging API
  slug: cayra-io-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-messaging-api-openapi.yml
- filename: cayra-io-mobile-invite-api-openapi.yml
  format: yaml
  label: Cayra Mobile Invite API
  slug: cayra-io-mobile-invite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-mobile-invite-api-openapi.yml
- filename: cayra-io-plaud-webhook-api-openapi.yml
  format: yaml
  label: Cayra Plaud Webhook API
  slug: cayra-io-plaud-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-plaud-webhook-api-openapi.yml
- filename: cayra-io-report-feedback-api-openapi.yml
  format: yaml
  label: Cayra Report Feedback API
  slug: cayra-io-report-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-report-feedback-api-openapi.yml
- filename: cayra-io-self-service-api-openapi.yml
  format: yaml
  label: Cayra Self Service API
  slug: cayra-io-self-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-self-service-api-openapi.yml
- filename: cayra-io-stripe-api-openapi.yml
  format: yaml
  label: Cayra Stripe API
  slug: cayra-io-stripe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-stripe-api-openapi.yml
- filename: cayra-io-stripe-webhook-api-openapi.yml
  format: yaml
  label: Cayra Stripe Webhook API
  slug: cayra-io-stripe-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-stripe-webhook-api-openapi.yml
- filename: cayra-io-usage-api-openapi.yml
  format: yaml
  label: Cayra Usage API
  slug: cayra-io-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-usage-api-openapi.yml
- filename: cayra-io-whatsapp-routing-api-openapi.yml
  format: yaml
  label: Cayra Whatsapp Routing API
  slug: cayra-io-whatsapp-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-whatsapp-routing-api-openapi.yml
- filename: cayra-io-whatsapp-webhook-api-openapi.yml
  format: yaml
  label: Cayra Whatsapp Webhook API
  slug: cayra-io-whatsapp-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-whatsapp-webhook-api-openapi.yml
consequence_counts:
  physical: 6
  read: 45
  safety-critical: 4
  write: 40
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Cayra Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/admin/licenses/{license_key}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/licenses/workspace/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/me/workspace/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/admin/provisioning/jobs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/me/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/me/credit-pack-checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/me/provisioning/jobs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/me/workspace/post-provision-confirmation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/messaging/whatsapp/send
operation_count: 95
overview: 'Cayra exposes 95 API operations that an AI agent could call, of which 50 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read, 40 write, 6 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cayra
provider_slug: cayra-io
slug: cayra-io-agentic-access
source_filename: cayra-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cayra-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 95\n  by_action_class:\n    connected: 45\n    acting: 50\n  by_consequence:\n    read: 45\n    write: 40\n    safety-critical: 4\n    physical: 6\n  human_in_the_loop_required: 4\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/customers\n\
  \  method: get\n  operationId: list_customers_api_v1_admin_customers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/customers\n  method: post\n  operationId: create_customer_api_v1_admin_customers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/customers/{customer_id}\n  method: patch\n  operationId: update_customer_api_v1_admin_customers__customer_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/admin/companies\n  method: get\n  operationId: list_companies_api_v1_admin_companies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/companies\n  method: post\n  operationId: create_company_api_v1_admin_companies_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/companies/{company_id}\n  method: patch\n  operationId: update_company_api_v1_admin_companies__company_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/licenses\n  method: post\n  operationId: generate_license_api_v1_admin_licenses_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/licenses\n  method: get\n  operationId: list_licenses_api_v1_admin_licenses_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/licenses/{license_key}\n  method: get\n  operationId: get_license_details_api_v1_admin_licenses__license_key__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/licenses/{license_key}/expiry\n\
  \  method: patch\n  operationId: update_license_expiry_api_v1_admin_licenses__license_key__expiry_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/licenses/{license_key}/provider-secrets\n  method: patch\n  operationId: update_license_provider_secrets_api_v1_admin_licenses__license_key__provider_secrets_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/licenses/{license_key}/revoke\n  method: post\n  operationId: revoke_license_api_v1_admin_licenses__license_key__revoke_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/admin/licenses/expiring-soon\n  method: get\n  operationId: get_licenses_expiring_soon_api_v1_admin_licenses_expiring_soon_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/billings\n  method: post\n  operationId: create_billing_api_v1_admin_billings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/billings\n\
  \  method: get\n  operationId: list_billings_api_v1_admin_billings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/billings/{billing_id}\n  method: get\n  operationId: get_billing_api_v1_admin_billings__billing_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/billings/{billing_id}\n  method: patch\n  operationId: update_billing_api_v1_admin_billings__billing_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/credit-events\n  method: post\n  operationId: create_credit_event_api_v1_admin_credit_events_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/credit-events\n  method: get\n  operationId: list_credit_events_api_v1_admin_credit_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/agreements\n  method: post\n  operationId: create_agreement_api_v1_admin_agreements_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/agreements\n  method: get\n  operationId: list_agreements_api_v1_admin_agreements_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/agreements/versions\n  method: post\n  operationId: create_agreement_version_api_v1_admin_agreements_versions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/agreements/versions\n  method: get\n  operationId: list_agreement_versions_api_v1_admin_agreements_versions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/agreements/acceptances\n  method: post\n  operationId: record_acceptance_api_v1_admin_agreements_acceptances_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/agreements/acceptances\n  method: get\n  operationId: list_acceptances_api_v1_admin_agreements_acceptances_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/profile\n  method: get\n  operationId: get_profile_api_v1_me_profile_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/profile\n  method: patch\n  operationId: update_profile_api_v1_me_profile_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/companies\n  method: get\n  operationId: list_companies_api_v1_me_companies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/companies\n  method: post\n  operationId: create_company_api_v1_me_companies_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/companies/{company_id}\n  method: patch\n  operationId: update_company_self_api_v1_me_companies__company_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/licenses\n  method: get\n  operationId: list_my_licenses_api_v1_me_licenses_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/billings\n  method: get\n  operationId: list_my_billings_api_v1_me_billings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/agreements\n  method: get\n  operationId: list_agreements_self_api_v1_me_agreements_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/agreements/versions\n  method: get\n  operationId:\
  \ list_agreement_versions_self_api_v1_me_agreements_versions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/agreements/acceptances\n  method: get\n  operationId: list_my_acceptances_api_v1_me_agreements_acceptances_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/agreements/acceptances\n  method: post\n  operationId: accept_agreement_self_api_v1_me_agreements_acceptances_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/usage/balance\n  method: get\n  operationId: get_my_usage_balance_api_v1_me_usage_balance_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/usage/daily\n  method: get\n  operationId: get_my_daily_usage_api_v1_me_usage_daily_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/packages\n  method: get\n  operationId: list_deployment_packages_self_api_v1_me_packages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/provisioning/active\n  method: get\n  operationId: get_active_provisioning_job_api_v1_me_provisioning_active_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/deployments/current\n  method: get\n  operationId:\
  \ get_current_deployment_api_v1_me_deployments_current_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/bootstrap\n  method: get\n  operationId: get_dashboard_bootstrap_api_v1_me_bootstrap_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/workspace/draft\n  method: patch\n  operationId: save_self_service_workspace_draft_api_v1_me_workspace_draft_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/provisioning/jobs\n  method: post\n  operationId: create_self_service_provisioning_job_api_v1_me_provisioning_jobs_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/workspace/reset\n  method: post\n  operationId: reset_self_service_workspace_api_v1_me_workspace_reset_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/me/workspace/post-provision-confirmation\n  method: post\n  operationId: complete_self_service_post_provision_confirmation_api_v1_me_workspace_post_provision_confirmation_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/provisioning/jobs/{job_id}\n  method: get\n  operationId: get_self_service_provisioning_job_api_v1_me_provisioning_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/redirect-session\n  method: post\n  operationId: create_redirect_session_api_v1_me_redirect_session_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/licenses/workspace/summary\n  method: get\n  operationId: get_workspace_summary_from_license_api_v1_licenses_workspace_summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/licenses/workspace/summary\n  method: patch\n  operationId: update_workspace_summary_from_license_api_v1_licenses_workspace_summary_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/licenses/workspace/deployment\n  method: get\n  operationId: get_workspace_deployment_from_license_api_v1_licenses_workspace_deployment_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/licenses/activate\n  method: post\n  operationId: activate_license_api_v1_licenses_activate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/licenses/heartbeat\n  method: post\n  operationId: license_heartbeat_api_v1_licenses_heartbeat_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/licenses/status\n  method: get\n  operationId: get_license_status_api_v1_licenses_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/licenses/redirect/consume\n  method: post\n  operationId: consume_redirect_token_api_v1_licenses_redirect_consume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/licenses/workspace/reset\n  method: post\n  operationId: reset_workspace_from_license_api_v1_licenses_workspace_reset_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/downloads/installer\n  method: post\n  operationId: download_installer_api_v1_downloads_installer_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/usage/events\n  method: post\n  operationId: record_usage_event_api_v1_usage_events_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/usage/balance\n  method: get\n  operationId: get_usage_balance_api_v1_usage_balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage/daily\n  method: get\n  operationId: get_daily_usage_api_v1_usage_daily_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/licenses/{license_key}/usage/events\n  method: post\n  operationId: record_usage_event_with_license_key_api_v1_licenses__license_key__usage_events_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/licenses/{license_key}/usage/balance\n  method: get\n  operationId: get_usage_balance_with_license_key_api_v1_licenses__license_key__usage_balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/licenses/{license_key}/usage/daily\n  method: get\n  operationId: get_daily_usage_with_license_key_api_v1_licenses__license_key__usage_daily_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/messaging/whatsapp/send\n  method: post\n  operationId: send_whatsapp_message_api_v1_messaging_whatsapp_send_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/messaging/whatsapp/status-callback\n  method: post\n  operationId: whatsapp_status_callback_api_v1_messaging_whatsapp_status_callback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/whatsapp/webhook/incoming\n  method: post\n  operationId: handle_incoming_whatsapp_api_v1_whatsapp_webhook_incoming_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/whatsapp-routing/register\n  method: post\n  operationId: register_agent_routing_api_v1_whatsapp_routing_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/whatsapp-routing/unregister\n  method: post\n  operationId: unregister_agent_routing_api_v1_whatsapp_routing_unregister_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/provisioning/jobs\n  method: post\n  operationId: create_provisioning_job_api_v1_admin_provisioning_jobs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/provisioning/jobs\n  method: get\n  operationId: list_provisioning_jobs_api_v1_admin_provisioning_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/admin/provisioning/jobs/{job_id}\n  method: get\n  operationId: get_provisioning_job_api_v1_admin_provisioning_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/provisioning/jobs/{job_id}/events\n  method: get\n  operationId: list_provisioning_job_events_api_v1_admin_provisioning_jobs__job_id__events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deployments\n  method: get\n  operationId: list_deployments_v1_deployments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deployments/{deployment_id}\n  method: get\n  operationId: get_deployment_v1_deployments__deployment_id__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deployments/{deployment_id}\n  method: delete\n  operationId: terminate_deployment_v1_deployments__deployment_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/deployments/{deployment_id}/audit-logs\n  method: get\n  operationId: get_deployment_audit_logs_v1_deployments__deployment_id__audit_logs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/report-feedback\n  method: post\n  operationId: report_feedback_api_v1_report_feedback_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/auth/invite\n  method: post\n  operationId: create_invite_api_v1_auth_invite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/auth/invite/qr-allocate\n  method: post\n  operationId: qr_allocate_invite_api_v1_auth_invite_qr_allocate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /api/v1/auth/invite/{token}\n  method: get\n  operationId: resolve_invite_api_v1_auth_invite__token__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/invite/mark-used\n  method: patch\n  operationId: mark_invite_used_api_v1_auth_invite_mark_used_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/subscription\n  method: get\n  operationId: get_subscription_api_v1_me_subscription_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/checkout\n  method: post\n\
  \  operationId: create_checkout_api_v1_me_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/billing-portal\n  method: post\n  operationId: create_billing_portal_api_v1_me_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/upgrade-preview\n  method: get\n  operationId: upgrade_preview_api_v1_me_upgrade_preview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/setup-intent\n  method: post\n  operationId: create_setup_intent_api_v1_me_setup_intent_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/credit-packs\n  method: get\n  operationId: list_credit_packs_api_v1_me_credit_packs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/credit-pack-checkout\n  method: post\n  operationId: create_credit_pack_checkout_api_v1_me_credit_pack_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/stripe/webhook\n  method: post\n  operationId: stripe_webhook_api_v1_stripe_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/vm-pool/status\n  method: get\n  operationId: get_vm_pool_status_api_v1_admin_vm_pool_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/vm-pool/replenish\n  method: post\n  operationId: trigger_vm_pool_replenish_api_v1_admin_vm_pool_replenish_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/vm-pool/retire/{pool_entry_id}\n  method: post\n  operationId: retire_pool_entry_api_v1_admin_vm_pool_retire__pool_entry_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/plaud/webhook\n  method: post\n  operationId: handle_plaud_webhook_api_v1_plaud_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n"
source_yaml_url: https://artifacts.apis.io/cayra-io/agentic-access/cayra-io-agentic-access.yml
summary_line: 95 operations · 50 acting · 4 human-in-the-loop
tags:
- Artificial Intelligence
- Enterprise
- Decision Intelligence
- ERP
- Database
---
