---
acting_count: 74
action_class_counts:
  acting: 74
  connected: 68
api_specs:
- filename: argorant-com-account-api-openapi.yml
  format: yaml
  label: Argorant Account API
  slug: argorant-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-account-api-openapi.yml
- filename: argorant-com-blocklist-api-openapi.yml
  format: yaml
  label: Argorant Blocklist API
  slug: argorant-com-blocklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-blocklist-api-openapi.yml
- filename: argorant-com-campaigns-api-openapi.yml
  format: yaml
  label: Argorant Campaigns API
  slug: argorant-com-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-campaigns-api-openapi.yml
- filename: argorant-com-companies-api-openapi.yml
  format: yaml
  label: Argorant Companies API
  slug: argorant-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-companies-api-openapi.yml
- filename: argorant-com-credits-api-openapi.yml
  format: yaml
  label: Argorant Credits API
  slug: argorant-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-credits-api-openapi.yml
- filename: argorant-com-email-finder-api-openapi.yml
  format: yaml
  label: Argorant Email finder API
  slug: argorant-com-email-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-email-finder-api-openapi.yml
- filename: argorant-com-enrich-api-openapi.yml
  format: yaml
  label: Argorant Enrich API
  slug: argorant-com-enrich-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-enrich-api-openapi.yml
- filename: argorant-com-exports-api-openapi.yml
  format: yaml
  label: Argorant Exports API
  slug: argorant-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-exports-api-openapi.yml
- filename: argorant-com-inbox-api-openapi.yml
  format: yaml
  label: Argorant Inbox API
  slug: argorant-com-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-inbox-api-openapi.yml
- filename: argorant-com-integrations-api-openapi.yml
  format: yaml
  label: Argorant Integrations API
  slug: argorant-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-integrations-api-openapi.yml
- filename: argorant-com-lists-api-openapi.yml
  format: yaml
  label: Argorant Lists API
  slug: argorant-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-lists-api-openapi.yml
- filename: argorant-com-lookups-api-openapi.yml
  format: yaml
  label: Argorant Lookups API
  slug: argorant-com-lookups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-lookups-api-openapi.yml
- filename: argorant-com-mailboxes-api-openapi.yml
  format: yaml
  label: Argorant Mailboxes API
  slug: argorant-com-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-mailboxes-api-openapi.yml
- filename: argorant-com-people-api-openapi.yml
  format: yaml
  label: Argorant People API
  slug: argorant-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-people-api-openapi.yml
- filename: argorant-com-verification-api-openapi.yml
  format: yaml
  label: Argorant Verification API
  slug: argorant-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-verification-api-openapi.yml
- filename: argorant-com-webhooks-api-openapi.yml
  format: yaml
  label: Argorant Webhooks API
  slug: argorant-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argorant-com/openapi/argorant-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 10
  read: 68
  safety-critical: 1
  write: 63
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Argorant Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/campaigns/{campaign_id}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/campaigns/{campaign_id}/senders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/campaigns/{campaign_id}/senders/{email}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/campaigns/{campaign_id}/test-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/credits/purchases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/inboxes/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/inboxes/orders/{order_id}/bundles/{bundle_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/inboxes/orders/{order_id}/domains/{domain}/renewal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/inboxes/orders/{order_id}/tags
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/integrations/{integration_id}/pushes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/webhooks/{webhook_id}/test
operation_count: 142
overview: 'Argorant exposes 142 API operations that an AI agent could call, of which 74 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 68 read, 63 write, 10 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Argorant
provider_slug: argorant-com
slug: argorant-com-agentic-access
source_filename: argorant-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/argorant-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 142\n  by_action_class:\n    connected: 68\n    acting: 74\n  by_consequence:\n    read: 68\n    write: 63\n    physical: 10\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1\n  method: get\n  operationId: api-index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  operationId: get-me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account\n\
  \  method: get\n  operationId: get-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credits/packs\n  method: get\n  operationId: list-credit-packs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credits/quote\n  method: post\n  operationId: quote-credits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/credits/purchases\n  method: post\n  operationId: buy-credits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n \
  \     exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/credits/purchases\n  method: get\n  operationId: list-credit-purchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credits/purchases/{purchase_id}\n  method: get\n  operationId: get-credit-purchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lookups/industries\n  method: get\n  operationId: lookup-industries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lookups/countries\n  method: get\n  operationId: lookup-countries\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lookups/keywords\n  method: get\n  operationId: lookup-keywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lookups/technologies\n  method: get\n  operationId: lookup-technologies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lookups/titles\n  method: get\n  operationId: lookup-titles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/people/count\n  method: get\n  operationId: count-people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/people/filters\n  method: get\n  operationId: people-filters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lookups/places\n  method: get\n  operationId: lookup-places\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/people/search\n  method: get\n  operationId: search-people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/people/reveal\n  method: post\n  operationId: reveal-people\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/people/phones\n  method: post\n  operationId: reveal-phones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/people/phones/pricing\n  method: get\n  operationId: phone-pricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/count\n  method: get\n  operationId: count-companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/search\n  method: get\n  operationId: search-companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{domain}/people\n  method:\
  \ get\n  operationId: company-people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/enrich\n  method: post\n  operationId: enrich\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/email-finder/pricing\n  method: get\n  operationId: email-finder-pricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/email-finder/find\n  method: post\n  operationId: find-email\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/email-finder/jobs\n\
  \  method: post\n  operationId: create-email-finder-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/email-finder/jobs\n  method: get\n  operationId: list-email-finder-jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/email-finder/jobs/{job_id}\n  method: get\n  operationId: get-email-finder-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/email-finder/jobs/{job_id}/results\n  method: get\n  operationId: get-email-finder-results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/email-finder/jobs/{job_id}/resume\n  method: post\n\
  \  operationId: resume-email-finder-job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/email-finder/jobs/{job_id}/cancel\n  method: post\n  operationId: cancel-email-finder-job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/email-finder/lookups\n  method: get\n  operationId: list-email-finder-lookups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verifications/quote\n  method: post\n  operationId:\
  \ quote-verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verifications\n  method: post\n  operationId: start-verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verifications/{run_id}\n  method: get\n  operationId: get-verification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lists\n  method: get\n  operationId: list-lists\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lists\n  method: post\n  operationId: create-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/lists/{list_id}/fill\n  method: get\n  operationId: list-fill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lists/{list_id}\n  method: get\n  operationId: get-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lists/{list_id}\n  method: patch\n  operationId: rename-list\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/lists/{list_id}\n  method: delete\n  operationId: delete-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/lists/{list_id}/people\n  method: get\n  operationId: list-people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lists/{list_id}/items\n  method: post\n  operationId: append-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/lists/{list_id}/export\n  method: post\n  operationId: export-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/exports\n  method: post\n  operationId: create-export\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/exports\n  method: get\n  operationId: list-exports\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/exports/{job_id}\n  method: get\n  operationId: get-export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/exports/{job_id}/download\n  method: get\n  operationId: download-export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/export-batches/{batch_id}\n  method: get\n  operationId: get-export-batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns\n  method: get\n  operationId: list-campaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/campaigns\n  method: post\n  operationId: create-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}\n  method: get\n  operationId: get-campaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}\n  method: patch\n  operationId: update-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}\n\
  \  method: delete\n  operationId: delete-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/duplicate\n  method: post\n  operationId: duplicate-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/emails\n  method: post\n  operationId: set-campaign-emails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/leads\n  method: post\n  operationId: add-campaign-leads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/leads\n  method: get\n  operationId: list-campaign-leads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}/leads/{email}\n  method: delete\n  operationId: remove-campaign-lead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/leads/remove\n  method: post\n  operationId: remove-campaign-leads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/leads/restore\n  method: post\n  operationId: restore-campaign-leads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/leads/move\n  method: post\n  operationId: move-campaign-leads\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/lead-jobs\n  method: get\n  operationId: list-campaign-lead-jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}/lead-jobs/{job_id}\n  method: get\n  operationId: get-campaign-lead-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}/leads/custom-fields\n  method: patch\n  operationId: set-lead-custom-fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/leads/custom-fields/import\n  method: post\n  operationId: import-lead-custom-fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/leads/custom-fields/import/{job_id}\n  method: get\n  operationId: get-lead-custom-fields-import\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}/personalization\n  method: get\n  operationId: get-campaign-personalization\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}/personalization\n  method: put\n  operationId: set-campaign-personalization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/senders\n  method: post\n  operationId: set-campaign-senders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/senders\n  method: get\n  operationId: list-campaign-senders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}/test-email\n  method: post\n  operationId: send-test-email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/folders\n  method: get\n  operationId: list-folders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/folders\n  method: post\n  operationId: create-folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/folders/{folder_id}\n  method: patch\n  operationId: rename-folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaign-tags\n  method: get\n  operationId: list-campaign-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaign-tags\n  method: post\n  operationId: tag-campaigns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/folder\n  method: post\n  operationId: move-campaign-to-folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/senders/{email}\n  method: delete\n  operationId: remove-campaign-sender\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/launch\n  method: post\n  operationId: launch-campaign\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/pause\n  method: post\n  operationId: pause-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/stop\n  method: post\n  operationId: stop-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/analytics\n  method: get\n  operationId: campaign-analytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}/replies\n  method: get\n  operationId: campaign-replies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}/subsequences\n  method: get\n  operationId: get-campaign-subsequences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/campaigns/{campaign_id}/subsequences\n  method: put\n  operationId: set-campaign-subsequences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/subsequences\n  method: post\n  operationId: set-campaign-subsequences-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/campaigns/{campaign_id}/subsequences/{subsequence_id}\n  method: patch\n  operationId: set-subsequence-enabled\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox\n\
  \  method: get\n  operationId: inbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/inbox/{event_id}\n  method: get\n  operationId: inbox-thread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/inbox/{event_id}/reply\n  method: post\n  operationId: inbox-reply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox/{event_id}/forward\n  method: post\n  operationId: inbox-forward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox/{event_id}/classify\n  method: post\n  operationId: inbox-classify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reply-statuses\n  method: get\n  operationId: reply-statuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reply-statuses\n  method: post\n  operationId: create-reply-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reply-statuses/{key}\n  method: patch\n  operationId: update-reply-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reply-statuses/{key}\n  method: delete\n  operationId: delete-reply-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/blocklist\n  method: get\n  operationId: list-blocklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /api/v1/blocklist\n  method: post\n  operationId: add-blocklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/blocklist/bulk\n  method: post\n  operationId: bulk-add-blocklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/blocklist/bulk-remove\n  method: post\n  operationId: bulk-remove-blocklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/blocklist/jobs/{job_id}\n  method: get\n  operationId: get-blocklist-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/blocklist/{entry_id}\n  method: delete\n  operationId: remove-blocklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inboxes\n  method: get\n  operationId: list-inboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/inboxes/{email}\n  method: patch\n  operationId: update-inbox\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inboxes/{email}\n  method: delete\n  operationId: delete-inbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inboxes/update\n  method: post\n  operationId: update-inboxes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inboxes/{email}/signature\n\
  \  method: get\n  operationId: get-inbox-signature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/inboxes/{email}/signature\n  method: put\n  operationId: set-inbox-signature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inboxes/{email}/signature\n  method: delete\n  operationId: delete-inbox-signature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (41 KB total) ---\n# Full\
  \ source: https://artifacts.apis.io/argorant-com/agentic-access/argorant-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/argorant-com/agentic-access/argorant-com-agentic-access.yml
summary_line: 142 operations · 74 acting · 1 human-in-the-loop
tags:
- B2B
- Data
- Email Verification
- Artificial Intelligence
- Outreach
- Software-as-a-Service
---
