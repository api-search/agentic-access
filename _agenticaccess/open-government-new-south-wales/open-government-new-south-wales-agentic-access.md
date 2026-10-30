---
acting_count: 0
action_class_counts:
  connected: 35
api_specs:
- filename: open-government-new-south-wales-browse-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Browse API
  slug: open-government-new-south-wales-browse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-browse-api-openapi.yml
- filename: open-government-new-south-wales-details-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Details API
  slug: open-government-new-south-wales-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-details-api-openapi.yml
- filename: open-government-new-south-wales-fuelcheckrefdata-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Fuel Check Ref Data API
  slug: open-government-new-south-wales-fuelcheckrefdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-fuelcheckrefdata-api-openapi.yml
- filename: open-government-new-south-wales-fuelpricecheck-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Fuel Price Check API
  slug: open-government-new-south-wales-fuelpricecheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-fuelpricecheck-api-openapi.yml
- filename: open-government-new-south-wales-pharmacyregister-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Pharmacyregister API
  slug: open-government-new-south-wales-pharmacyregister-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-pharmacyregister-api-openapi.yml
- filename: open-government-new-south-wales-security-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Security API
  slug: open-government-new-south-wales-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-security-api-openapi.yml
- filename: open-government-new-south-wales-verify-api-openapi.yml
  format: yaml
  label: Open Government, New South Wales Verify API
  slug: open-government-new-south-wales-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/openapi/open-government-new-south-wales-verify-api-openapi.yml
consequence_counts:
  read: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Open Government New South Wales Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 35
overview: 'Open Government, New South Wales exposes 35 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Open Government, New South Wales
provider_slug: open-government-new-south-wales
slug: open-government-new-south-wales-agentic-access
source_filename: open-government-new-south-wales-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/open-government-new-south-wales-fuel-openapi.yml, openapi/open-government-new-south-wales-home-building-compensation-openapi.yml,\n  openapi/open-government-new-south-wales-pharmacy-register-openapi.yml, openapi/open-government-new-south-wales-property-openapi.yml,\n  openapi/open-government-new-south-wales-security-openapi.yml, openapi/open-government-new-south-wales-trades-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 35\n  by_consequence:\n    read: 35\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/client_credential/accesstoken\n  method: get\n  operationId: OauthClientCredentialAccesstokenGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelCheckRefData/v1/fuel/lovs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelCheckRefData/v2/fuel/lovs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v1/fuel/prices/location\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v2/fuel/prices/location\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v1/fuel/prices/nearby\n  method:\
  \ post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v2/fuel/prices/nearby\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v1/fuel/prices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v2/fuel/prices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v1/fuel/prices/new\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v2/fuel/prices/new\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v1/fuel/prices/station/{stationCode}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FuelPriceCheck/v2/fuel/prices/station/{stationCode}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/client_credential/accesstoken\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hbccheckregister/v1/browse\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /hbccheckregister/v1/verify\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hbccheckregister/v1/details\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/client_credential/accesstoken\n  method: get\n  operationId: OauthClientCredentialAccesstokenGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pharmacyregister/v1/browse\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pharmacyregister/v1/verify\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pharmacyregister/v1/details\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pharmacyregister/v1/licence/search/query\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pharmacyregister/v1/licence/search/details/pharmacy/{licenceId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/client_credential/accesstoken\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyregister/v1/browse\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyregister/v1/verify\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /propertyregister/v1/details\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/client_credential/accesstoken\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /securityregister/v1/browse\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /securityregister/v1/verify\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /securityregister/v1/details\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/client_credential/accesstoken\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tradesregister/v1/browse\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tradesregister/v1/verify\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tradesregister/v1/details\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/agentic-access/open-government-new-south-wales-agentic-access.yml
summary_line: 35 operations
tags:
- Government
- Public APIs
- Open Data
- Australia
- New South Wales
- Public Sector
- Fuel Prices
---
