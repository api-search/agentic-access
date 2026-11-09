---
acting_count: 47
action_class_counts:
  acting: 47
  connected: 17
consequence_counts:
  physical: 3
  read: 17
  safety-critical: 14
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 14
kind: agentic-access
layout: agentic-access
method: generated
name: Hubject Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /charging/v21/operators/{operatorID}/authorize/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /charging/v21/operators/{operatorID}/authorize/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /charging/v21/providers/{externalID}/authorize-remote/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /charging/v21/providers/{providerID}/authorize-remote/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reservation/v11/providers/{providerID}/reservation-stop-request
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reservation/v11/providers/{providerID}/reservation-stop-request
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/ccp/signedContractData
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/ccp/signedContractData/{emaid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/ccp/signedContractData/{pcid}/{emaid}/default
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/cps/forward/signedContractData
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/cps/generate/signedContractData
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/cps/signedContractData
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/oem/provCerts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/oem/provCerts/{pcid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cdrmgmt/v22/operators/{operatorID}/charge-detail-record
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cdrmgmt/v22/operators/{operatorID}/charge-detail-record
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cdrmgmt/v22/providers/{providerID}/get-charge-detail-records-request
operation_count: 64
overview: 'Hubject exposes 64 API operations that an AI agent could call, of which 47 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 30 write, 3 physical, and 14 safety-critical.


  14 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hubject
provider_slug: hubject
slug: hubject-agentic-access
source_filename: hubject-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/hubject-ngp-cpo-evse-swagger.json, openapi/hubject-ngp-cpo-service-offers-swagger.json,\n  openapi/hubject-ngp-emp-contracts-swagger.json, openapi/hubject-oicp-cpo-2.3-openapi.yml,\n  openapi/hubject-oicp-emp-2.3-openapi.yml, openapi/hubject-opcp-accesstoken-openapi.json, openapi/hubject-opcp-ccp-openapi.json,\n  openapi/hubject-opcp-cps-openapi.json, openapi/hubject-opcp-est-openapi.json, openapi/hubject-opcp-pcp-openapi.json,\n  openapi/hubject-opcp-rcp-openapi.json, openapi/hubject-opcp-webhooks-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 64\n  by_action_class:\n    acting: 47\n    connected: 17\n  by_consequence:\n    write: 30\n    read: 17\n    safety-critical:\
  \ 14\n    physical: 3\n  human_in_the_loop_required: 14\noperations:\n- path: /api/evsenetwork/v1/operators/{externalOperatorId}/network\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/evsenetwork/v1/operators/{externalOperatorId}/networks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partner/v1/operators/{externalID}/service-offers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partner/v1/operators/{externalID}/service-offers/attachments\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partner/v1/operators/{externalID}/service-offers/info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partner/v1/operators/{externalID}/service-offers/{serviceOfferId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partner/v1/operators/{externalID}/service-offers/{serviceOfferId}/historical-versions-info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/premium/contracts/v1/providers/{providerId}/operators/{operatorId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/premium/contracts/v1/providers/{providerId}/operators/{operatorId}/service-offers/{serviceOfferId}/networks/{networkId}/groups/{groupId}/evses\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charging/v21/operators/{operatorID}/authorize/start\n\
  \  method: post\n  operationId: eRoamingAuthorizeStart_v2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charging/v21/operators/{operatorID}/authorize/stop\n  method: post\n  operationId: eRoamingAuthorizeStop_V2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /charging/v21/providers/{providerID}/authorize-remote/start\n  method: post\n  operationId: eRoamingAuthorizeRemoteStart_v2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charging/v21/providers/{providerID}/authorize-remote/stop\n  method: post\n  operationId: eRoamingAuthorizeRemoteStop_v2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cdrmgmt/v22/operators/{operatorID}/charge-detail-record\n  method: post\n  operationId: eRoamingChargeDetailRecord_V2.2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservation/v11/providers/{providerID}/reservation-start-request\n  method: post\n  operationId: eRoamingAuthorizeRemoteReservationStart_V1.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservation/v11/providers/{providerID}/reservation-stop-request\n  method: post\n  operationId: eRoamingAuthorizeRemoteReservationStop_V1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /evsepush/v23/operators/{operatorID}/data-records\n\
  \  method: post\n  operationId: eRoamingPushEvseData_V2.3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evsepush/v21/operators/{operatorID}/status-records\n  method: post\n  operationId: eRoamingPushEvseStatus_V2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dynamicpricing/v10/operators/{operatorID}/pricing-products\n  method: post\n  operationId: eRoamingPushPricingProductData_V1.0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dynamicpricing/v10/operators/{operatorID}/evse-pricing\n  method: post\n  operationId: eRoamingPushEVSEPricing_V1.0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notificationmgmt/v11/charging-notifications\n  method: post\n  operationId: eRoamingChargingNotifications_V1.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charging/v21/operators/{operatorID}/authorize/start\n\
  \  method: post\n  operationId: eRoamingAuthorizeStart_v2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charging/v21/operators/{operatorID}/authorize/stop\n  method: post\n  operationId: eRoamingAuthorizeStop_V2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /charging/v21/providers/{providerID}/authorize-remote/start\n  method: post\n  operationId: eRoamingAuthorizeRemoteStart_v2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charging/v21/providers/{externalID}/authorize-remote/stop\n  method: post\n  operationId: eRoamingAuthorizeRemoteStop_v2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cdrmgmt/v22/operators/{operatorID}/charge-detail-record\n  method: post\n  operationId: eRoamingChargeDetailRecord_V2.2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdrmgmt/v22/providers/{providerID}/get-charge-detail-records-request\n  method: post\n  operationId: eRoamingGetChargeDetailRecords_V2.2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authdata/v21/providers/{providerID}/push-request\n  method: post\n  operationId: eRoamingPushAuthenticationData_V2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservation/v11/providers/{providerID}/reservation-start-request\n\
  \  method: post\n  operationId: eRoamingAuthorizeRemoteReservationStart_V1.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservation/v11/providers/{providerID}/reservation-stop-request\n  method: post\n  operationId: eRoamingAuthorizeRemoteReservationStop_V1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /evsepull/v23/providers/{providerID}/data-records\n  method: post\n  operationId: eRoamingPullEvseData_V2.3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evsepull/v21/providers/{providerID}/status-records\n  method: post\n  operationId: eRoamingPullEvseStatus_V2.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dynamicpricing/v10/providers/{providerID}/pricing-products\n  method: post\n  operationId: eRoamingPullPricingProductData_V1.0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /dynamicpricing/v10/providers/{providerID}/evse-pricing\n  method: post\n  operationId: eRoamingPullEVSEPricing_V1.0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notificationmgmt/v11/charging-notifications\n  method: post\n  operationId: eRoamingChargingNotifications_V1.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: issue-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ccp/signedContractData\n  method: post\n  operationId: getSignedContractData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ccp/signedContractData\n  method: put\n  operationId: addSignedContractData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/ccp/signedContractData/{emaid}\n  method: delete\n  operationId: deleteSignedContractData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/ccp/provideSignedContractData/{emaid}/{pcid}\n  method: get\n  operationId: provideSignedContractData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ccp/signedContractData/{pcid}/{emaid}/default\n  method: post\n  operationId: setDefaultContract\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/ccp/lookupContract/{emaid}\n  method: get\n  operationId: lookupContract\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ccp/signedContractData/{pcid}\n  method: get\n  operationId: getContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cps/contractData/signed\n  method: put\n  operationId: put-v1-cps-signContractData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cps/forward/signedContractData\n  method: put\n  operationId: createAndForwardSignedContractData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n \
  \     exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/cps/signedContractData\n  method: put\n  operationId: createSignedContractData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/cps/generate/signedContractData\n  method: put\n  operationId: generateSignedContractData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cps/signer\n\
  \  method: get\n  operationId: get-cps-signer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/est/{ca}/simpleenroll/{iso-version}\n  method: post\n  operationId: simpleenroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{ca}/cacerts/{iso-version}/{algorithm}/\n  method: get\n  operationId: cacerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oem/provCerts/{pcid}\n  method: get\n  operationId: getOEMProvCert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v1/oem/provCerts/{pcid}\n  method: delete\n  operationId: deleteOEMProvCert\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/oem/provCerts\n  method: put\n  operationId: addOEMProvCert\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/oem/provCerts/lookupVehicle/{pcid}\n  method: get\n  operationId: lookupVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/root/rootCerts/{rootCertificateId}\n  method: get\n  operationId: getRootCert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/root/rootCerts/{rootCertificateId}\n  method: delete\n  operationId: delete-v1-root-rootCerts-rootCertificateId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/root/rootCerts\n  method: get\n  operationId: getAllRootCerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/root/rootCerts\n  method: put\n  operationId: put-v1-root-rootCerts\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/root/ctl\n  method: get\n  operationId: get-v1-root-ctl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/endpoints\n  method: post\n  operationId: create-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/endpoints\n  method: get\n  operationId: get-webhook-endpoints\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/endpoints/{id}\n  method: get\n  operationId: get-webhook-endpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/endpoints/{id}\n  method: put\n  operationId: update-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/endpoints/{id}\n  method: delete\n  operationId: delete-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/hubject/agentic-access/hubject-agentic-access.yml
summary_line: 64 operations · 47 acting · 14 human-in-the-loop
tags:
- Company
- E-Mobility
- EV Charging
- Interoperability
---
