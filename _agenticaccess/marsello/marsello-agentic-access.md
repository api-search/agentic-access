---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 46
api_specs:
- filename: marsello-account-api-openapi.yml
  format: yaml
  label: Marsello Account API
  slug: marsello-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-account-api-openapi.yml
- filename: marsello-activities-api-openapi.yml
  format: yaml
  label: Marsello Activities API
  slug: marsello-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-activities-api-openapi.yml
- filename: marsello-apps-api-openapi.yml
  format: yaml
  label: Marsello Apps API
  slug: marsello-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-apps-api-openapi.yml
- filename: marsello-checkins-api-openapi.yml
  format: yaml
  label: Marsello Check Ins API
  slug: marsello-checkins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-checkins-api-openapi.yml
- filename: marsello-customerdisplayactivecustomer-api-openapi.yml
  format: yaml
  label: Marsello Customer Display Active Customer API
  slug: marsello-customerdisplayactivecustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-customerdisplayactivecustomer-api-openapi.yml
- filename: marsello-customerdisplaysettings-api-openapi.yml
  format: yaml
  label: Marsello Customer Display Settings API
  slug: marsello-customerdisplaysettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-customerdisplaysettings-api-openapi.yml
- filename: marsello-customers-api-openapi.yml
  format: yaml
  label: Marsello Customers API
  slug: marsello-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-customers-api-openapi.yml
- filename: marsello-devices-api-openapi.yml
  format: yaml
  label: Marsello Devices API
  slug: marsello-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-devices-api-openapi.yml
- filename: marsello-orderdumps-api-openapi.yml
  format: yaml
  label: Marsello Order Dumps API
  slug: marsello-orderdumps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-orderdumps-api-openapi.yml
- filename: marsello-orders-api-openapi.yml
  format: yaml
  label: Marsello Orders API
  slug: marsello-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-orders-api-openapi.yml
- filename: marsello-rewards-api-openapi.yml
  format: yaml
  label: Marsello Rewards API
  slug: marsello-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-rewards-api-openapi.yml
- filename: marsello-stores-api-openapi.yml
  format: yaml
  label: Marsello Stores API
  slug: marsello-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/openapi/marsello-stores-api-openapi.yml
consequence_counts:
  physical: 12
  read: 46
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Marsello Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/stores/{storeId}/order-dumps/{posType}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/stores/{storeId}/order-dumps/{posType}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/stores/{storeId}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/stores/{storeId}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/stores/{storeId}/orders/{sourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/stores/{storeId}/orders/{sourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/stores/{storeId}/order-dumps/{posType}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/stores/{storeId}/order-dumps/{posType}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/stores/{storeId}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/stores/{storeId}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/stores/{storeId}/orders/{sourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/stores/{storeId}/orders/{sourceId}
operation_count: 90
overview: 'Marsello exposes 90 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read, 32 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Marsello
provider_slug: marsello
slug: marsello-agentic-access
source_filename: marsello-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/marsello-loyalty-api-v1.json, openapi/marsello-loyalty-api-v2.json, openapi/provider-v1.json,\n  openapi/provider-v2.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 90\n  by_action_class:\n    connected: 46\n    acting: 44\n  by_consequence:\n    read: 46\n    write: 32\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/account\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n\
  \    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}/activities\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}/activities\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}/activities/{activityType}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/activities/{customerId}/{token}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/stores/{storeId}/check-ins\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n\
  \    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/email/{email}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n\
  \    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/stores/{storeId}/devices\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/stores/{storeId}/order-dumps/{posType}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/stores/{storeId}/orders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n\
  \    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/stores/{storeId}/orders/{sourceId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/stores/{storeId}/customers/{customerId}/rewards/{rewardId}\n\
  \  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/stores/{storeId}/customers/{customerId}/rewards/{rewardId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  \    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/stores\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/stores/{storeId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/account\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/account/providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/account/token-info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customers/{customerId}/activities\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customers/{customerId}/activities\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n\
  \    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customers/{customerId}/activities/{activityType}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/activities/{customerId}/{token}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    -\
  \ https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/apps/windows/{fileName}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores/{storeId}/check-ins\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customer-display-active-customer/{customerDisplayDeviceId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n  \
  \  - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customer-display-active-customer/update/{customerDisplayDeviceId}/customer/{customerId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/account/customerdisplaysettings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customers/{customerId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customers/{customerId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customers/email/{email}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n  \
  \  - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/customers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n\
  \    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores/{storeId}/devices\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores/{storeId}/order-dumps/{posType}\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores/{storeId}/orders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores/{storeId}/orders/{sourceId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n\
  \    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores/{storeId}/customers/{customerId}/rewards/{rewardId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores/{storeId}/customers/{customerId}/rewards/{rewardId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores/{storeId}/customers/{customerId}/coupons/{rewardId}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n\
  \    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v2/stores/{storeId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n\
  \    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/account\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}/activities\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n\
  \    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}/activities\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}/activities/{activityType}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/activities/{customerId}/{token}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n\
  \    - write:orders\n    - write:rewards\n- path: /v1/stores/{storeId}/check-ins\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n\
  \    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/{customerId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers/email/{email}\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n- path: /v1/customers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://dev.marsello.com/scope/read.all\n    - https://dev.marsello.com/scope/write.all\n    - read:account\n    - read:activities\n    - read:customers\n    - read:orders\n    - read:rewards\n    - read:stores\n    - write:activities\n    - write:customers\n    - write:devices\n    - write:orders\n    - write:rewards\n\n\n# --- truncated at 32 KB (52 KB total)\
  \ ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/agentic-access/marsello-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marsello/refs/heads/main/agentic-access/marsello-agentic-access.yml
summary_line: 90 operations · 44 acting
tags:
- Loyalty
- Marketing
- Retail
- Hospitality
- Platform
---
