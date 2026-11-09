---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 41
api_specs:
- filename: recruitmcp-com-account-api-openapi.yml
  format: yaml
  label: recruitmcp-com Account API
  slug: recruitmcp-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-account-api-openapi.yml
- filename: recruitmcp-com-billing-api-openapi.yml
  format: yaml
  label: recruitmcp-com Billing API
  slug: recruitmcp-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-billing-api-openapi.yml
- filename: recruitmcp-com-companies-api-openapi.yml
  format: yaml
  label: recruitmcp-com Companies API
  slug: recruitmcp-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-companies-api-openapi.yml
- filename: recruitmcp-com-contacts-api-openapi.yml
  format: yaml
  label: recruitmcp-com Contacts API
  slug: recruitmcp-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-contacts-api-openapi.yml
- filename: recruitmcp-com-customers-api-openapi.yml
  format: yaml
  label: recruitmcp-com Customers API
  slug: recruitmcp-com-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-customers-api-openapi.yml
- filename: recruitmcp-com-events-api-openapi.yml
  format: yaml
  label: recruitmcp-com Events API
  slug: recruitmcp-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-events-api-openapi.yml
- filename: recruitmcp-com-lists-api-openapi.yml
  format: yaml
  label: recruitmcp-com Lists API
  slug: recruitmcp-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-lists-api-openapi.yml
- filename: recruitmcp-com-privacy-api-openapi.yml
  format: yaml
  label: recruitmcp-com Privacy API
  slug: recruitmcp-com-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-privacy-api-openapi.yml
- filename: recruitmcp-com-profiles-api-openapi.yml
  format: yaml
  label: recruitmcp-com Profiles API
  slug: recruitmcp-com-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-profiles-api-openapi.yml
- filename: recruitmcp-com-search-api-openapi.yml
  format: yaml
  label: recruitmcp-com Search API
  slug: recruitmcp-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-search-api-openapi.yml
consequence_counts:
  physical: 5
  read: 41
  safety-critical: 3
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Recruitmcp Com Agentic Access
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
  path: /v1/billing/auto-refill
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/privacy/opt-out
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/developer/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/subscriptions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhook-endpoints/{endpoint_id}/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/workspaces/verify/resend
operation_count: 85
overview: 'recruitmcp-com exposes 85 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 read, 36 write, 5 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: recruitmcp-com
provider_slug: recruitmcp-com
slug: recruitmcp-com-agentic-access
source_filename: recruitmcp-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/recruitmcp-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 85\n  by_action_class:\n    acting: 44\n    connected: 41\n  by_consequence:\n    write: 36\n    physical: 5\n    read: 41\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signup\n  method: post\n  operationId: signupWorkspace\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/verify\n  method: post\n  operationId: verifyWorkspaceEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/verify/resend\n  method: post\n  operationId: resendWorkspaceVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/workspaces/recover\n  method: post\n  operationId: requestKeyRecovery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/recover/link\n  method: post\n  operationId: describeKeyRecovery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspaces/recover/confirm\n  method: post\n  operationId: confirmKeyRecovery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspace\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace\n  method: patch\n  operationId: updateWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys/{key_id}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/subscription/plan\n  method: post\n  operationId: changeSubscriptionPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/auto-refill\n  method: get\n  operationId: getAutoRefill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/auto-refill\n  method: put\n  operationId: updateAutoRefill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/auto-refill\n  method: delete\n  operationId: disableAutoRefill\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - billing:manage\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/billing/developer\n  method: get\n  operationId: getDeveloperBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/developer\n  method: patch\n  operationId: updateDeveloperSpendLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - billing:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/developer/checkout\n  method: post\n  operationId: createDeveloperCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - billing:manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/transactions\n  method: get\n  operationId: listBillingTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookups/locations\n  method: get\n  operationId: lookupLocations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookups/areas\n  method: get\n  operationId: lookupArea\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookups/companies\n  method: get\n  operationId: lookupCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies:resolve\n  method: post\n  operationId: resolveCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lookups/industries\n  method: get\n  operationId: listIndustries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookups/seniorities\n  method: get\n  operationId: listSeniorities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookups/experience-ranges\n  method: get\n  operationId: listExperienceRanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookups/functions\n  method: get\n  operationId: listFunctions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookups/languages\n  method: get\n  operationId: listProfileLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookups/headcounts\n  method: get\n  operationId: listCompanyHeadcounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people/search\n  method: post\n  operationId: searchPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:spend\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people/{profile_id}\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people/{profile_id}\n  method: delete\n  operationId: erasePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - privacy:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people:enrich\n  method: post\n  operationId: enrichPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people:fetch\n  method: post\n  operationId: fetchPeople\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:spend\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people:match\n  method: post\n  operationId: matchPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people/{profile_id}/contacts\n  method: get\n  operationId: getPersonContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - contacts:spend\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people/{profile_id}/contacts\n  method: post\n  operationId: lookupPersonContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - contacts:spend\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/people/{profile_id}/contacts\n  method: delete\n  operationId: deletePersonContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - privacy:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/people/contacts:fetch\n  method: post\n  operationId: lookupContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - contacts:spend\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/jobs/{job_id}\n  method: get\n  operationId: getContactJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - contacts:spend\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media/{token}\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/seen\n  method: get\n  operationId: listSeen\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/seen\n  method: post\n\
  \  operationId: upsertSeen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lists:write\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/seen:check\n  method: post\n  operationId: checkSeen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sourcing:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/seen/{seen_id}\n  method: get\n  operationId: getSeenEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/seen/{seen_id}\n\
  \  method: patch\n  operationId: updateSeenEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lists:write\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/seen/{seen_id}\n  method: delete\n  operationId: deleteSeenEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lists:write\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists\n  method: get\n  operationId: listLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/lists\n  method: post\n  operationId: createList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lists:write\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists/{list_id}\n  method: get\n  operationId: getList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lists/{list_id}\n  method: patch\n  operationId: updateList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lists:write\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists/{list_id}\n  method: delete\n  operationId: deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lists:write\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists/{list_id}/items\n  method: get\n  operationId: listListItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lists/{list_id}/items\n  method: post\n  operationId: addListItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lists:write\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists/{list_id}/items/{item_id}\n  method: delete\n  operationId: removeListItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - lists:write\n    - sourcing:spend\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists/{list_id}/export\n  method: get\n  operationId: exportList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/erasures\n  method: post\n  operationId: createErasure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - privacy:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/suppressions\n  method: get\n  operationId: listSuppressions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sourcing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/suppressions\n  method: post\n  operationId: createSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - privacy:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/suppressions/{suppression_id}\n  method: delete\n  operationId: deleteSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - privacy:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/privacy/cache\n  method: delete\n  operationId: deleteCaches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - privacy:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/privacy/opt-out\n  method: post\n  operationId: requestOptOut\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /v1/privacy/opt-out/confirm\n  method: get\n  operationId: confirmOptOut\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{event_id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-endpoints\n\
  \  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints/{endpoint_id}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-endpoints/{endpoint_id}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/webhook-endpoints/{endpoint_id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints/{endpoint_id}/rotate-secret\n  method: post\n  operationId: rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints/{endpoint_id}/test\n  method: post\n  operationId: testWebhookEndpoint\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account:manage\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/recruitmcp-com/agentic-access/recruitmcp-com-agentic-access.yml
summary_line: 85 operations · 44 acting · 3 human-in-the-loop
tags:
- Company
- Recruiting
- MCP
- Human Resources
---
