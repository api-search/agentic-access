---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 43
api_specs:
- filename: petexec-authentication-api-openapi.yml
  format: yaml
  label: PetExec Authentication API
  slug: petexec-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-authentication-api-openapi.yml
- filename: petexec-boarding-api-openapi.yml
  format: yaml
  label: PetExec Boarding API
  slug: petexec-boarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-boarding-api-openapi.yml
- filename: petexec-calendar-api-openapi.yml
  format: yaml
  label: PetExec Calendar API
  slug: petexec-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-calendar-api-openapi.yml
- filename: petexec-company-api-openapi.yml
  format: yaml
  label: PetExec Company API
  slug: petexec-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-company-api-openapi.yml
- filename: petexec-credit-cards-api-openapi.yml
  format: yaml
  label: PetExec Credit Cards API
  slug: petexec-credit-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-credit-cards-api-openapi.yml
- filename: petexec-daycare-api-openapi.yml
  format: yaml
  label: PetExec Daycare API
  slug: petexec-daycare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-daycare-api-openapi.yml
- filename: petexec-grooming-api-openapi.yml
  format: yaml
  label: PetExec Grooming API
  slug: petexec-grooming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-grooming-api-openapi.yml
- filename: petexec-owners-api-openapi.yml
  format: yaml
  label: PetExec Owners API
  slug: petexec-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-owners-api-openapi.yml
- filename: petexec-pets-api-openapi.yml
  format: yaml
  label: PetExec Pets API
  slug: petexec-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-pets-api-openapi.yml
- filename: petexec-profile-api-openapi.yml
  format: yaml
  label: PetExec Profile API
  slug: petexec-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-profile-api-openapi.yml
- filename: petexec-purchase-history-api-openapi.yml
  format: yaml
  label: PetExec Purchase History API
  slug: petexec-purchase-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-purchase-history-api-openapi.yml
- filename: petexec-reports-api-openapi.yml
  format: yaml
  label: PetExec Reports API
  slug: petexec-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-reports-api-openapi.yml
- filename: petexec-scheduled-services-api-openapi.yml
  format: yaml
  label: PetExec Scheduled Services API
  slug: petexec-scheduled-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-scheduled-services-api-openapi.yml
- filename: petexec-vaccinations-api-openapi.yml
  format: yaml
  label: PetExec Vaccinations API
  slug: petexec-vaccinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-vaccinations-api-openapi.yml
consequence_counts:
  read: 43
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Petexec Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 51
overview: 'PetExec exposes 51 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 43 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PetExec
provider_slug: petexec
slug: petexec-agentic-access
source_filename: petexec-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/petexec-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    acting: 8\n    connected: 43\n  by_consequence:\n    write: 8\n    read: 43\n  human_in_the_loop_required: 0\noperations:\n- path: /token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /owner\n  method: get\n  operationId: listOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /owner/{owner_id}\n  method: get\n  operationId: getOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/owners/{search_criteria}/page/{page_number}/data/{data_per_page}\n  method: get\n  operationId: searchOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pet/{pet_id}\n  method: get\n  operationId: getPet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pet/{pet_id}\n  method: delete\n  operationId: deletePet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pet-type/\n  method: get\n  operationId: listPetTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breed/pet-type/{pet_type_id}\n  method: get\n  operationId: listBreedsForPetType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/pets/{search_criteria}/page/{page_number}/data/{data_per_page}\n  method: get\n  operationId: searchPets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vet/\n  method: get\n  operationId: listVets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /boarding/{boarding_id}\n  method: get\n  operationId: getBoarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boarding/{boarding_id}\n  method: delete\n  operationId: deleteFutureBoarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boarding/packages/owner/{owner_id}\n  method: get\n  operationId: getOwnerBoardingPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boarding/services\n  method: get\n  operationId: listBoardingServices\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /daycare/{daycare_id}\n  method: get\n  operationId: getDaycare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /daycare/{daycare_id}\n  method: delete\n  operationId: deleteFutureDaycare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /daycare/services/\n  method: get\n  operationId: listDaycareServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grooming/{grooming_id}\n  method: get\n  operationId: getGrooming\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grooming/{grooming_id}\n  method: delete\n  operationId: deleteFutureGrooming\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /grooming/groomers\n  method: get\n  operationId: listGroomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grooming/services/\n  method: get\n  operationId: listGroomingServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-service/{scheduled_service_id}\n  method: delete\n  operationId:\
  \ deleteFutureScheduledService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduled-service/service-types/\n  method: get\n  operationId: listScheduledServiceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-service/services/\n  method: get\n  operationId: listScheduledServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduled-service/services/{service_type_id}\n  method: get\n  operationId: listServicesByServiceType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/boarding/start/{start_date}/end/{end_date}\n  method: get\n  operationId: getCompanyBoardingsScheduled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/daycare/start/{start_date}/end/{end_date}\n  method: get\n  operationId: getCompanyDaycaresScheduled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/grooming/start/{start_date}/end/{end_date}\n  method: get\n  operationId: getCompanyGroomingsScheduled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/scheduled-service/start/{start_date}/end/{end_date}\n  method: get\n  operationId: getCompanyScheduledServicesScheduled\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/owner/{owner_id}/boarding/start/{start_date}/end/{end_date}\n  method: get\n  operationId: getOwnerBoardingsScheduled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/owner/{owner_id}/daycare/start/{start_date}/end/{end_date}\n  method: get\n  operationId: getOwnerDaycaresScheduled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/owner/{owner_id}/grooming/start/{start_date}/end/{end_date}\n  method: get\n  operationId: getOwnerGroomingsScheduled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/owner/{owner_id}/scheduled-service/start/{start_date}/end/{end_date}\n\
  \  method: get\n  operationId: getOwnerScheduledServicesScheduled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shot/{shot_id}\n  method: get\n  operationId: getShot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shot/{shot_id}\n  method: delete\n  operationId: deleteShot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shot/pet-type/{pet_id}\n  method: get\n  operationId: getShotsForPetType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /user-card/owner/{owner_id}\n  method: get\n  operationId: getOwnerCreditCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-card/{card_id}/owner/{owner_id}\n  method: get\n  operationId: getOwnerCreditCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userCard/{card_id}\n  method: delete\n  operationId: deleteCreditCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase-history/owner/{owner_id}\n  method: get\n  operationId: getPurchaseHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/billing-report/{start_date}/{end_date}/{pay_type}/{owner_portal}\n  method: get\n  operationId: getBillingReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/statistics-report/{start_date}/{end_date}/{taxable_only}\n  method: get\n  operationId: getStatisticsReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/statistics-report/{start_date}/{end_date}/breakdown/{pay_type}\n  method: get\n  operationId: getStatisticsReportByPayType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/statistics-report/{start_date}/{end_date}/breakdown/service/{service_id}\n  method:\
  \ get\n  operationId: getStatisticsReportByServiceType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/locations\n  method: get\n  operationId: getCompanyLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/employees/\n  method: get\n  operationId: getCompanyEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/how-found/\n  method: get\n  operationId: getAllHowFound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /preference\n  method: get\n  operationId: getAllCompanyPreferences\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /preference/{preference_name}\n  method: get\n  operationId: getCompanyPreferenceValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/\n  method: get\n  operationId: getAuthenticatedUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu\n  method: get\n  operationId: getMenu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/agentic-access/petexec-agentic-access.yml
summary_line: 51 operations · 8 acting
tags:
- Pet Care
- Boarding
- Daycare
- Grooming
- Training
- Business Management
- Pet Business Software
---
