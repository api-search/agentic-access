---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 21
api_specs:
- filename: nextdc-comments-api-openapi.yml
  format: yaml
  label: NEXTDC Comments API
  slug: nextdc-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-comments-api-openapi.yml
- filename: nextdc-discount-api-openapi.yml
  format: yaml
  label: NEXTDC Discount API
  slug: nextdc-discount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-discount-api-openapi.yml
- filename: nextdc-discounts-api-openapi.yml
  format: yaml
  label: NEXTDC Discounts API
  slug: nextdc-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-discounts-api-openapi.yml
- filename: nextdc-limitations-api-openapi.yml
  format: yaml
  label: NEXTDC Limitations API
  slug: nextdc-limitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-limitations-api-openapi.yml
- filename: nextdc-locations-api-openapi.yml
  format: yaml
  label: NEXTDC Locations API
  slug: nextdc-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-locations-api-openapi.yml
- filename: nextdc-pricepoints-api-openapi.yml
  format: yaml
  label: NEXTDC Pricepoints API
  slug: nextdc-pricepoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-pricepoints-api-openapi.yml
- filename: nextdc-quote-api-openapi.yml
  format: yaml
  label: NEXTDC Quote API
  slug: nextdc-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-quote-api-openapi.yml
- filename: nextdc-quotes-api-openapi.yml
  format: yaml
  label: NEXTDC Quotes API
  slug: nextdc-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-quotes-api-openapi.yml
- filename: nextdc-resource-api-openapi.yml
  format: yaml
  label: NEXTDC Resource API
  slug: nextdc-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-resource-api-openapi.yml
- filename: nextdc-resources-api-openapi.yml
  format: yaml
  label: NEXTDC Resources API
  slug: nextdc-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-resources-api-openapi.yml
- filename: nextdc-service-api-openapi.yml
  format: yaml
  label: NEXTDC Service API
  slug: nextdc-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-service-api-openapi.yml
- filename: nextdc-services-api-openapi.yml
  format: yaml
  label: NEXTDC Services API
  slug: nextdc-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-services-api-openapi.yml
- filename: nextdc-task-api-openapi.yml
  format: yaml
  label: NEXTDC Task API
  slug: nextdc-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-task-api-openapi.yml
- filename: nextdc-tasks-api-openapi.yml
  format: yaml
  label: NEXTDC Tasks API
  slug: nextdc-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/openapi/nextdc-tasks-api-openapi.yml
consequence_counts:
  read: 21
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nextdc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 43
overview: 'NEXTDC exposes 43 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 22 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NEXTDC
provider_slug: nextdc
slug: nextdc-agentic-access
source_filename: nextdc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: generated\nsource: openapi/nextdc-axon-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 21\n    acting: 22\n  by_consequence:\n    read: 21\n    write: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/comments/{guid}\n  method: get\n  operationId: bizApiCommentCommentsBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations\n  method: get\n  operationId: bizApiLocationLocationsBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/locations/DCI\n  method: get\n  operationId: bizApiLocationLocationsDciBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations/PROVIDERS\n  method: get\n  operationId: bizApiLocationProvidersLocationsBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/limitations/{type}/{guid}\n  method: get\n  operationId: bizApiLimitationsRetrieveLimitationsBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resources/{company_id}/DISCOVER\n  method: get\n  operationId: bizApiResourceResourceDiscoverBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resources\n\
  \  method: get\n  operationId: bizApiResourceResourcesBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resource/PROVIDERS\n  method: get\n  operationId: bizApiResourceAvailableProvidersBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resource/TYPES\n  method: get\n  operationId: bizApiResourceRetrieveResourceAvailableTypesBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resource/{company_id}\n  method: post\n  operationId: bizApiResourceAllocateResourceBiz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resource/{resource_guid}\n  method: delete\n  operationId: bizApiResourceUnallocateResourceBiz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resource/customer/{resource_guid}\n  method: put\n  operationId: bizApiResourceUpdateCustomerResourceBiz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resource/LAG/{resource_guid}\n  method: put\n  operationId: bizApiLagResourceUpdateLagResourceBiz\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resource/LAG/{resource_guid}/{lag_resource_guid}\n  method: put\n  operationId: bizApiLagResourceUpdateAssociateLagResourceBiz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/service/{service_guid}\n  method: get\n  operationId: bizApiServiceServiceBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services\n  method: get\n  operationId: bizApiServiceServicesBiz\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{company_id}/{resource_guid}/DISCOVER\n  method: get\n  operationId: bizApiServiceServicesDiscoverBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/service/exc/{service_guid}/{diverse_service_guid}/INFO/DIVERSE\n  method: get\n  operationId: bizApiServiceIsDiverseBiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/service/exc/{service_guid}/{diverse_service_guid}/INFO/DIVERSE\n  method: put\n  operationId: bizApiServiceServiceUpdateDiversityBiz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/service/exc/{company_id}\n  method: post\n  operationId: bizApiServiceServiceCreateBiz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/service/exc/{service_guid}\n  method: put\n  operationId: bizApiServiceServiceUpdateBiz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/service/exc/{service_guid}\n  method: delete\n  operationId: bizApiServiceRemoveServiceBiz\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/service/exc/{service_guid}/APPROVAL\n  method: put\n  operationId: bizApiServiceApproveBiz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/service/exc/{service_guid}/INFO/DIVERSE\n  method: delete\n  operationId: bizApiServiceServiceDeleteDiversityBiz\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/tasks\n  method: get\n  operationId: bizApiTaskTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/{task_list_guid}\n  method: get\n  operationId: bizApiTaskTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/{task_list_guid}\n  method: put\n  operationId: bizApiTaskRunTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/discounts\n  method: get\n  operationId: bizApiDiscountsDiscounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/discount/{discount_guid}\n  method: delete\n  operationId: bizApiDiscountsRemoveDiscountCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/discount\n  method: post\n  operationId: bizApiDiscountsCreateDiscountCodeResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pricepoints\n  method: get\n  operationId: bizApiPricePointsPricePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/quotes\n  method: get\n  operationId: bizApiQuotesQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quote/{quote_guid}\n  method: get\n  operationId: bizApiQuotesQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quote/{quote_guid}\n  method: delete\n  operationId: bizApiQuotesRemoveQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quote/{quote_guid}\n  method: put\n  operationId: bizApiQuotesUpdateQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quote/{quote_guid}/render\n  method: get\n  operationId: bizApiQuotesQuoteRender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quote/{quote_guid}/pricepoints\n  method: get\n  operationId: bizApiQuotesQuotePricepoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quote\n  method: post\n  operationId: bizApiQuotesCreateQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/quote/{quote_guid}/ITEMADD\n  method: post\n  operationId: bizApiQuotesQuoteItemAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quote/{quote_guid}/item/{quote_item_guid}\n  method: put\n  operationId: bizApiQuotesQuoteItemUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quote/{quote_guid}/{quote_item_guid}/ITEMREMOVE\n  method: delete\n  operationId: bizApiQuotesQuoteItemRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quote/{quote_guid}/DUPLICATE\n  method: post\n  operationId: bizApiQuotesDuplicateQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quote/{quote_guid}/SUBMIT\n  method: put\n  operationId: bizApiQuotesSubmitQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextdc/refs/heads/main/agentic-access/nextdc-agentic-access.yml
summary_line: 43 operations · 22 acting
tags:
- Company
- Data Centers
- Colocation
- Cloud Infrastructure
- Connectivity
- Artificial Intelligence
- Australia
---
