---
acting_count: 145
action_class_counts:
  acting: 145
  connected: 66
api_specs:
- filename: spotnana-auth-openapi-original.json
  format: json
  label: Spotnana Authentication API
  slug: spotnana-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-auth-openapi-original.json
- filename: spotnana-users-openapi-original.json
  format: json
  label: Spotnana Users API
  slug: spotnana-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-users-openapi-original.json
- filename: spotnana-company-openapi-original.json
  format: json
  label: Spotnana Company API
  slug: spotnana-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-company-openapi-original.json
- filename: spotnana-policy-openapi-original.json
  format: json
  label: Spotnana Policy API
  slug: spotnana-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-policy-openapi-original.json
- filename: spotnana-trip-openapi-original.json
  format: json
  label: Spotnana Trip API
  slug: spotnana-trip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-trip-openapi-original.json
- filename: spotnana-air-openapi-original.json
  format: json
  label: Spotnana Air API
  slug: spotnana-air-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-air-openapi-original.json
- filename: spotnana-hotel-openapi-original.json
  format: json
  label: Spotnana Hotel API
  slug: spotnana-hotel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-hotel-openapi-original.json
- filename: spotnana-event-openapi-original.json
  format: json
  label: Spotnana Event API
  slug: spotnana-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-event-openapi-original.json
- filename: spotnana-template-openapi-original.json
  format: json
  label: Spotnana Event Template API
  slug: spotnana-event-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-template-openapi-original.json
- filename: spotnana-payments-openapi-original.json
  format: json
  label: Spotnana Payments API
  slug: spotnana-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-payments-openapi-original.json
- filename: spotnana-document-openapi-original.json
  format: json
  label: Spotnana Document API
  slug: spotnana-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/openapi/spotnana-document-openapi-original.json
consequence_counts:
  physical: 14
  read: 66
  safety-critical: 2
  write: 129
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Spotnana Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/api-users/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/companies/{companyId}/partner-public-keys/{kid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/air/flight-checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/events/{eventId}/invite/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/events/{eventId}/invite/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/invoicing/invoice-data
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/license/company/{companyId}/service-charge/per-trip
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payment/users/{userId}/payment-sources
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/payment/users/{userId}/payment-sources/{paymentSourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/payment/users/{userId}/payment-sources/{paymentSourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/service-charge/{entityType}/{entityId}/types/{type}/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/service-charge/{entityType}/{entityId}/types/{type}/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/trips/{tripId}/pnrs/{pnrId}/download-invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/users/{userId}/membership-info
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/air/company-transferable-unused-credits/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/tenant-encryption/{companyId}/key
operation_count: 211
overview: 'Spotnana exposes 211 API operations that an AI agent could call, of which 145 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 66 read, 129 write, 14 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spotnana
provider_slug: spotnana
slug: spotnana-agentic-access
source_filename: spotnana-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/spotnana-air-openapi-original.json, openapi/spotnana-auth-openapi-original.json,\n  openapi/spotnana-company-openapi-original.json, openapi/spotnana-document-openapi-original.json,\n  openapi/spotnana-event-openapi-original.json, openapi/spotnana-hotel-openapi-original.json,\n  openapi/spotnana-payments-openapi-original.json, openapi/spotnana-policy-openapi-original.json,\n  openapi/spotnana-template-openapi-original.json, openapi/spotnana-trip-openapi-original.json,\n  openapi/spotnana-users-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 211\n  by_action_class:\n    connected: 66\n    acting: 145\n  by_consequence:\n    read: 66\n    write: 129\n    physical:\
  \ 14\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v2/air-autocomplete\n  method: get\n  operationId: airAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/air/search-flights\n  method: post\n  operationId: airSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/flight-attributes\n  method: post\n  operationId: airAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/air/selected-itinerary\n  method: post\n  operationId: airSelectedItinerary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/loyalty-programs\n  method: get\n  operationId: getAirApplicableLoyalties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/air/airlines-info\n  method: get\n  operationId: getAirlinesInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/air/flight-checkout\n  method: post\n  operationId: airFlightCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/seat-map\n  method: post\n  operationId: airSeatMap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/initiate-booking\n  method: post\n  operationId: airInitiateBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/revalidate-itinerary\n  method:\
  \ post\n  operationId: airRevalidateItinerary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/intermediate-revalidate-itinerary\n  method: post\n  operationId: airIntermediateRevalidateItinerary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/create-pnr\n  method: post\n  operationId: airCreatePnr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/cancel-pnr\n  method: post\n  operationId: airCancelPnr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/pnrs/{pnrId}/exchange-details\n  method: get\n  operationId: getAirPnrExchangeDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/air/modify-search\n  method: post\n  operationId: airModifySearchV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /v2/air/modify-book\n  method: post\n  operationId: airModifyBookV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/pnrs/{pnrId}/update\n  method: post\n  operationId: airPnrEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/air/special-service-requests\n  method: get\n  operationId: getSpecialServiceRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/air/special-service-requests/categories\n\
  \  method: get\n  operationId: getSpecialServiceRequestsFilterByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/air/fare-rules/fetch\n  method: post\n  operationId: fetchAirFareRules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/air/fetch-traveler-unused-credits\n  method: post\n  operationId: fetchTravelerUnusedCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/air/company-unused-credits/list\n\
  \  method: post\n  operationId: fetchCompanyUnusedCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/air/company-transferable-unused-credits/list\n  method: post\n  operationId: fetchCompanyTransferableUnusedCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/air/company-credits/migrations\n  method: post\n  operationId: migrateUnusedCreditsInCompanyCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/oauth2-token\n  method: post\n  operationId: fetchOauth2Token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/api-users\n  method: post\n  operationId: createApiUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/api-users\n  method: get\n  operationId: getApiUsers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/api-users/revoke\n  method: post\n  operationId: deleteApiUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/api-users/rotate\n  method: post\n  operationId: rotateClientSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies\n  method: post\n  operationId: createCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}\n  method: get\n  operationId: readCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}\n  method: put\n  operationId: updateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}\n\
  \  method: delete\n  operationId: deleteCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/legal-entities\n  method: post\n  operationId: createLegalEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/legal-entities\n  method: get\n  operationId: listLegalEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/legal-entities/{legalEntityId}\n\
  \  method: get\n  operationId: getLegalEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/legal-entities/{legalEntityId}\n  method: put\n  operationId: updateLegalEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/legal-entities/{legalEntityId}\n  method: delete\n  operationId: deleteLegalEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/cost-centers\n\
  \  method: post\n  operationId: createCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/cost-centers\n  method: get\n  operationId: listCostCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/cost-centers/{costCenterId}\n  method: get\n  operationId: getCostCenter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/cost-centers/{costCenterId}\n  method: put\n  operationId: updateCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/cost-centers/{costCenterId}\n  method: delete\n  operationId: deleteCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/companies/{companyId}/cost-centers/list\n  method: post\n  operationId: listCostCentersV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/legal-entities/{legalEntityId}/offices\n\
  \  method: post\n  operationId: createOffice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/legal-entities/{legalEntityId}/offices\n  method: get\n  operationId: listLegalEntityOffices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/office-list\n  method: post\n  operationId: listOfficesV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/legal-entities/{legalEntityId}/offices/{officeId}\n\
  \  method: get\n  operationId: getOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/legal-entities/{legalEntityId}/offices/{officeId}\n  method: put\n  operationId: updateOffice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/legal-entities/{legalEntityId}/offices/{officeId}\n  method: delete\n  operationId: deleteOffice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/companies/{companyId}/partner-public-keys\n  method: post\n  operationId: addPartnerPublicKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/partner-public-keys\n  method: get\n  operationId: listPartnerPublicKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/partner-public-keys/{kid}\n  method: delete\n  operationId: revokePartnerPublicKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n  \
  \  escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/companies/{companyId}/departments\n  method: post\n  operationId: createDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/departments\n  method: get\n  operationId: listDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/departments/{departmentId}\n  method: get\n  operationId: getDepartment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/departments/{departmentId}\n\
  \  method: put\n  operationId: updateDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/departments/{departmentId}\n  method: delete\n  operationId: deleteDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/companies/{companyId}/departments/list\n  method: post\n  operationId: listDepartmentsV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/grades\n  method: post\n  operationId: createGrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/grades/{gradeId}\n  method: get\n  operationId: getGrade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/grades/{gradeId}\n  method: put\n  operationId: updateGrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/grades/{gradeId}\n  method: delete\n  operationId: deleteGrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/grades/list\n  method: post\n  operationId: listGrades\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/features\n  method: get\n  operationId: getCompanyFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/features\n  method: patch\n  operationId: updateCompanyFeaturesPatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/travel-content-config\n  method: get\n  operationId: getCompanyTravelContentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/travel-content-config\n  method: put\n  operationId: updateCompanyTravelContentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/travel-content-config\n  method: delete\n  operationId: deleteCompanyTravelContentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/white-label-config\n  method: put\n  operationId: updateCompanyWhiteLabelConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/white-label-config\n  method: get\n  operationId: getCompanyWhiteLabelConfig\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/white-label-config\n  method: delete\n  operationId: deleteCompanyWhiteLabelConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/managers-config\n  method: put\n  operationId: updateCompanyManagersConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/managers-config\n  method: get\n  operationId: getCompanyManagersConfig\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/managers-config\n  method: delete\n  operationId: deleteCompanyManagersConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/license/company/{companyId}/service-charge/per-trip\n  method: get\n  operationId: getCompanyPerTripSrvCharge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/license/company/{companyId}/service-charge/per-trip\n  method: post\n  operationId: setCompanyPerTripSrvCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/service-charge/{entityType}/{entityId}/types/{type}/list\n  method: post\n  operationId: listServiceCharges\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/enrollment-config\n  method: put\n  operationId: updateCompanyEnrollmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/enrollment-config\n  method: get\n  operationId: getCompanyEnrollmentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/color-config\n  method: put\n  operationId: updateColorConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/color-config\n  method: get\n  operationId: getColorConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/tier-config\n\
  \  method: put\n  operationId: updateCompanyTierConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/tier-config\n  method: get\n  operationId: getCompanyTierConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/stealth-config\n  method: put\n  operationId: updateCompanyStealthConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/stealth-config\n\
  \  method: get\n  operationId: getCompanyStealthConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/companies/{companyId}/vendor-preferences\n  method: post\n  operationId: uploadCompanyPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/preference-tiers\n  method: put\n  operationId: storePreferenceTiers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{companyId}/preference-tiers\n\
  \  method: get\n  operationId: listPreferenceTiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/tenant-encryption/{companyId}/key\n  method: post\n  operationId: provisionOrRotateTenantKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/documents\n\
  \  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/{documentId}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/{documentId}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/events\n  method: post\n  operationId: createEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/events/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/events/{eventId}\n  method: delete\n  operationId: deleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/events/read-by-external-id\n  method: get\n  operationId: getEventByExternalID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \n\n# --- truncated at 32 KB (67 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/agentic-access/spotnana-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotnana/refs/heads/main/agentic-access/spotnana-agentic-access.yml
summary_line: 211 operations · 145 acting · 2 human-in-the-loop
tags:
- Company
- Travel
- Corporate Travel
- Travel Management
- Booking
- Air
- Hotel
- Payments
- Travel as a Service
---
