---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 30
api_specs:
- filename: jaggaer-async-api-openapi.yml
  format: yaml
  label: JAGGAER Async API
  slug: jaggaer-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-async-api-openapi.yml
- filename: jaggaer-attributes-api-openapi.yml
  format: yaml
  label: JAGGAER Attributes API
  slug: jaggaer-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-attributes-api-openapi.yml
- filename: jaggaer-awards-api-openapi.yml
  format: yaml
  label: JAGGAER Awards API
  slug: jaggaer-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-awards-api-openapi.yml
- filename: jaggaer-bids-api-openapi.yml
  format: yaml
  label: JAGGAER Bids API
  slug: jaggaer-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-bids-api-openapi.yml
- filename: jaggaer-contacts-api-openapi.yml
  format: yaml
  label: JAGGAER Contacts API
  slug: jaggaer-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-contacts-api-openapi.yml
- filename: jaggaer-customer-hosts-api-openapi.yml
  format: yaml
  label: JAGGAER Customer Hosts API
  slug: jaggaer-customer-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-customer-hosts-api-openapi.yml
- filename: jaggaer-events-api-openapi.yml
  format: yaml
  label: JAGGAER Events API
  slug: jaggaer-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-events-api-openapi.yml
- filename: jaggaer-items-api-openapi.yml
  format: yaml
  label: JAGGAER Items API
  slug: jaggaer-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-items-api-openapi.yml
- filename: jaggaer-jobs-api-openapi.yml
  format: yaml
  label: JAGGAER Jobs API
  slug: jaggaer-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-jobs-api-openapi.yml
- filename: jaggaer-locations-api-openapi.yml
  format: yaml
  label: JAGGAER Locations API
  slug: jaggaer-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-locations-api-openapi.yml
- filename: jaggaer-rates-api-openapi.yml
  format: yaml
  label: JAGGAER Rates API
  slug: jaggaer-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-rates-api-openapi.yml
- filename: jaggaer-scenarios-api-openapi.yml
  format: yaml
  label: JAGGAER Scenarios API
  slug: jaggaer-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-scenarios-api-openapi.yml
- filename: jaggaer-suppliers-api-openapi.yml
  format: yaml
  label: JAGGAER Suppliers API
  slug: jaggaer-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-suppliers-api-openapi.yml
- filename: jaggaer-templates-api-openapi.yml
  format: yaml
  label: JAGGAER Templates API
  slug: jaggaer-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-templates-api-openapi.yml
- filename: jaggaer-uploads-api-openapi.yml
  format: yaml
  label: JAGGAER Uploads API
  slug: jaggaer-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-uploads-api-openapi.yml
- filename: jaggaer-users-api-openapi.yml
  format: yaml
  label: JAGGAER Users API
  slug: jaggaer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-users-api-openapi.yml
consequence_counts:
  read: 30
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jaggaer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 50
overview: 'JAGGAER exposes 50 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read and 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: JAGGAER
provider_slug: jaggaer
slug: jaggaer-agentic-access
source_filename: jaggaer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/jaggaer-aso-ches-openapi.yml, openapi/jaggaer-aso-ees-openapi.yml, openapi/jaggaer-aso-quay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    connected: 30\n    acting: 20\n  by_consequence:\n    read: 30\n    write: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /asyncStatus/{encoded-async-pid}\n  method: get\n  operationId: getAsyncStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chost/{customer-host-id}/fqdn\n  method: get\n  operationId: getCustomerHostFqdn\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chost/{customer-host-id}/user/{user-id}/template/{template-id}/apiEvent\n  method: post\n  operationId: createEventFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chost/{customer-host-id}/user/{user-id}/template/{template-id}/apiEvent/async\n  method: post\n  operationId: createEventFromTemplateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chost/{customer-host-id}/user/{user-id}/apiEvents\n  method: get\n  operationId:\
  \ getEventsByUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chost/{customer-host-id}/apiLocationNames\n  method: get\n  operationId: getLocationNames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chost/{customer-host-id}/templateType/{template-type-id}/apiSubcategories\n  method: get\n  operationId: getSubcategoriesByTemplateType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chost/{customer-host-id}/user/{user-id}/apiTemplates\n  method: get\n  operationId: getTemplatesByUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chost/{customer-host-id}/apiTemplateTypes\n\
  \  method: get\n  operationId: getTemplateTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chost/{customer-host-id}/apiUser/{user-id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chost/{customer-host-id}/apiUsers\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asyncStatus/{encoded-async-pid}\n  method: get\n  operationId: getAsyncStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiAttribute/{attribute-id}\n  method: get\n  operationId: getAttribute\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiAttribute/{attribute-id}\n  method: patch\n  operationId: updateAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/apiAttribute/{attribute-id}\n  method: delete\n  operationId: deleteAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/apiAttributes\n  method: get\n  operationId: getAttributes\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiAttributes\n  method: post\n  operationId: createAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/apiAttributes\n  method: patch\n  operationId: updateAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/attributeType/{attribute-type}/apiAttributes\n  method: get\n  operationId: getAttributesByType\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/scenario/preferred/apiAwards/async\n  method: get\n  operationId: getAwardsByPreferredScenarioAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/scenario/{scenario-id}/apiAwards/async\n  method: get\n  operationId: getAwardsByScenarioAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiBids/async\n  method: get\n  operationId: getBidsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/bidRound/{bid-round}/apiBids/async\n  method: get\n  operationId: getBidsByBidRoundAsync\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiContact/{contact-id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiContact/{contact-id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/user/{user-id}/apiContact/{contact-id}\n  method: patch\n  operationId: updateContactByUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/user/{user-id}/apiContacts\n  method: patch\n  operationId: updateContactsByUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/supplier/{supplier-id}/apiContacts\n  method: get\n  operationId: getContactsBySupplier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/user/{user-id}/supplier/{supplier-id}/apiContacts\n  method: post\n  operationId: createContactByUserAndSupplier\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/apiItem/{item-id}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiItem/{item-id}\n  method: delete\n  operationId: deleteItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/user/{user-id}/apiItem/{item-id}\n  method: patch\n  operationId: updateItemByUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/apiItems\n  method: get\n  operationId: getItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiItems/async\n  method: get\n  operationId: getItemsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/user/{user-id}/apiItems\n  method: post\n  operationId: createItemsByUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /event/{event-id}/user/{user-id}/apiItems\n  method: patch\n  operationId: updateItemsByUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/apiRate/{rate-id}\n  method: get\n  operationId: getRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiRates/async\n  method: get\n  operationId: getRatesAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiScenarios\n  method: get\n  operationId: getScenarios\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiSupplier/{supplier-id}\n  method: get\n  operationId: getSupplier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/apiSupplier/{supplier-id}\n  method: delete\n  operationId: deleteSupplier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/user/{user-id}/apiSupplier/{supplier-id}\n  method: patch\n  operationId: updateSupplierByUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/apiSuppliers\n  method: get\n  operationId: getSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{event-id}/user/{user-id}/apiSuppliers\n  method: post\n  operationId: createSuppliersByUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/user/{user-id}/apiSuppliers\n  method: patch\n  operationId: updateSuppliersByUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event/{event-id}/user/{user-id}/entity/{entity}/uploadUrl\n  method: get\n  operationId: getUploadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submitJob\n  method: post\n  operationId: submitJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancelJob/{job-id}\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /jobStatus/{job-id}\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/{job-id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/agentic-access/jaggaer-agentic-access.yml
summary_line: 50 operations · 20 acting
tags:
- Procurement
- Sourcing
- Supplier Management
- Contracts
- Spend Analytics
- eProcurement
- Source-to-Pay
- Procure-to-Pay
---
