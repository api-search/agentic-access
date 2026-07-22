---
acting_count: 226
action_class_counts:
  acting: 226
  connected: 270
api_specs:
- filename: nfon-pbx-configuration-api-openapi.json
  format: json
  label: NFON PBX Configuration API
  slug: nfon-pbx-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/openapi/nfon-pbx-configuration-api-openapi.json
- filename: nfon-cti-api-openapi.yml
  format: yaml
  label: NFON CTI API
  slug: nfon-cti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/openapi/nfon-cti-api-openapi.yml
- filename: nfon-call-history-api-openapi.yml
  format: yaml
  label: NFON Call History API
  slug: nfon-call-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/openapi/nfon-call-history-api-openapi.yml
- filename: nfon-service-portal-api.postman_collection.json
  format: json
  label: NFON Service Portal API (legacy)
  slug: nfon-service-portal-api-legacy
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/postman/nfon-service-portal-api.postman_collection.json
consequence_counts:
  read: 270
  safety-critical: 20
  write: 206
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 20
kind: agentic-access
layout: agentic-access
method: generated
name: Nfon Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tenants/{participantExternalIdentifier}/devices/{uniqueIdentifier}/reset-authentication
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/skills
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/skills/login-status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tenants/{participantExternalIdentifier}/targets/skill-services
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}/destination-on-rejection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}/inbound-trunk-numbers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}/inbound-trunk-numbers/{didNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}/members
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}/members/{extensionNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}/members/{extensionNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}/timeout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /tenants/{participantExternalIdentifier}/targets/skill-services/{serviceNumber}/timeout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tenants/{participantExternalIdentifier}/targets/time-control-services
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /tenants/{participantExternalIdentifier}/targets/time-control-services/{serviceNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /tenants/{participantExternalIdentifier}/targets/time-control-services/{serviceNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tenants/{participantExternalIdentifier}/targets/time-control-services/{serviceNumber}/inbound-trunk-numbers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /tenants/{participantExternalIdentifier}/targets/time-control-services/{serviceNumber}/inbound-trunk-numbers/{didNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /tenants/{tenant}/stop-trial-period
operation_count: 496
overview: 'Nfon exposes 496 API operations that an AI agent could call, of which 226 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 270 read, 206 write, and 20 safety-critical.


  20 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nfon
provider_slug: nfon
slug: nfon-agentic-access
source_filename: nfon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/nfon-call-history-api-openapi.yml, openapi/nfon-cti-api-openapi.yml, openapi/nfon-pbx-configuration-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 496\n  by_action_class:\n    connected: 270\n    acting: 226\n  by_consequence:\n    read: 270\n    write: 206\n    safety-critical: 20\n  human_in_the_loop_required: 20\noperations:\n- path: /records\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /records/{uuid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records/{uuid}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /login\n  method: put\n  operationId: refreshAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/jwks.json\n  method: get\n  operationId: publicKeyWellKnown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extensions/phone/data\n  method: get\n  operationId: getPhoneExtensionData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extensions/phone/states\n  method: get\n  operationId: getState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /extensions/phone/calls\n  method: post\n  operationId: originate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extensions/phone/calls\n  method: get\n  operationId: stream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extensions/phone/calls/{uuid}\n  method: delete\n  operationId: cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountSalesForceId}/sites/{siteSalesforceId}\n\
  \  method: get\n  operationId: get_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountSalesForceId}/sites/{siteSalesforceId}\n  method: put\n  operationId: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract-types\n  method: get\n  operationId: get_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contract-types/{contractType}\n  method: get\n  operationId: get_4\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - tenant.admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{oldID}/replace/{newID}\n  method: put\n  operationId: replaceSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bss.license-manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant}/virtual-fax-extensions/bulk\n  method: get\n  operationId: bulkExportVirtualFaxExtensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant}/virtual-fax-extensions/bulk\n  method: post\n  operationId: bulkImportVirtualFaxExtensions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{siteId}\n  method: delete\n  operationId: deleteSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bss.license-manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant}\n  method: patch\n  operationId: updateTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bss.license-manage\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant}/billing-extensions\n  method: post\n  operationId: createBillingExtensions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bss.license-manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /directcall-numbers/{number}\n  method: get\n  operationId: get_202\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant}/clip-screened-prefixes\n  method: post\n  operationId: createClipScreenedPrefix\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - bss.license-manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration-types\n  method: get\n  operationId: get_203\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration-types\n  method: post\n  operationId: post_54\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /integration-types/{integrationId}\n  method: put\n  operationId: put_56\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration-types/{integrationId}\n  method: delete\n  operationId: delete_56\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integration-types/{integrationId}\n  method: get\n  operationId: get_204\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/contracts\n  method: get\n  operationId: get_31\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/contracts\n  method: post\n  operationId: post_5\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/voice-recording-profiles/{voiceRecordingProfileId}\n\
  \  method: get\n  operationId: get_194\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operatorId}\n  method: get\n  operationId: get_206\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operatorId}\n  method: put\n  operationId: put_57\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/targets/group-services/available-destinations-on-timeout\n\
  \  method: get\n  operationId: get_176\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/frontdesk-services/{serviceNumber}/target/{targetServiceNumber}\n  method: put\n  operationId: updateTargetByTargetId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/targets/frontdesk-services/{serviceNumber}/target/{targetServiceNumber}\n  method: delete\n  operationId:\
  \ deleteTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/targets/frontdesk-services/{serviceNumber}/target/{targetServiceNumber}\n  method: get\n  operationId: getTargetByTargetId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions\n  method: get\n  operationId: get_66\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions\n  method: post\n  operationId: post_15\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/codec-profiles\n  method: get\n  operationId: get_26\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/default-system-integrator\n  method: get\n  operationId: get_11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/default-system-integrator\n  method: put\n  operationId: put_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.operator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/targets/skill-services\n  method: get\n  operationId: get_138\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/skill-services\n  method: post\n  operationId: post_44\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/targets/ivr-services/available-general-announcements\n  method: get\n  operationId: get_112\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n\
  \    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operatorId}/pbx-groups/{pbxGroupName}\n  method: get\n  operationId: get_211\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.operator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/devices/{deviceType}/{baseId}/license-keys\n  method: get\n  operationId: get_40\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/devices/{deviceType}/{baseId}/license-keys\n  method: post\n  operationId: post_11\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/available-internal-outgoings\n  method: get\n  operationId: get_64\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/call-forwards\n  method: get\n  operationId: get_78\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n\
  \    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/call-forwards\n  method: put\n  operationId: put_24\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/devices/{deviceType}/{deviceId}\n  method: put\n  operationId: put_16\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/devices/{deviceType}/{deviceId}\n  method: delete\n  operationId: delete_12\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/devices/{deviceType}/{deviceId}\n  method: get\n  operationId: get_47\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}\n  method: get\n  operationId: get_13\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/devices/{deviceType}/{deviceId}/site-options\n  method: put\n  operationId: put_13\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/devices/{deviceType}/{deviceId}/site-options\n\
  \  method: delete\n  operationId: delete_8\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/devices/{deviceType}/{deviceId}/site-options\n  method: get\n  operationId: get_44\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operatorId}/rating-profiles\n  method: get\n  operationId: get_213\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - tenant.admin\n    - tenant.operator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operatorId}/rating-profiles\n  method: post\n  operationId: post_55\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/callforward-globals\n  method: get\n  operationId: get_70\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/callforward-globals\n\
  \  method: put\n  operationId: put_18\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/announcements/{id}\n  method: put\n  operationId: simplePut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/announcements/{id}\n  method:\
  \ delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/announcements/{id}\n  method: get\n  operationId: getContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/callforward-globals/{type}\n  method: get\n  operationId: get_71\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/callforward-globals/{type}\n  method: put\n  operationId: put_19\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/callforward-globals/{type}/available\n  method: get\n  operationId: getAvailable_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: get\n  operationId: get_200\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operatorId}/rating-profiles/available\n  method: get\n  operationId: get_212\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/callforward-profiles/{profileNumber}/rules\n  method: get\n  operationId: get_74\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    -\
  \ tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/callforward-profiles/{profileNumber}/rules\n  method: post\n  operationId: post_18\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operatorId}/rating-profiles/{ratingProfileName}\n  method: delete\n  operationId: delete_57\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operatorId}/rating-profiles/{ratingProfileName}\n  method: get\n  operationId: get_214\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.operator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/callforward-profiles/{profileNumber}/rules/{sourceId}/{type}/available\n  method: get\n  operationId: getAvailable_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/devices\n  method: get\n  operationId: get_60\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/devices\n  method: post\n  operationId: post_13\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operators/{operatorId}/tenants\n  method: get\n  operationId: get_209\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.operator\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/function-keys/available-targets\n  method: get\n  operationId: get_80\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/function-keys/{keyNumber}\n  method: put\n  operationId: put_25\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/function-keys/{keyNumber}\n  method: delete\n  operationId: delete_19\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/function-keys/{keyNumber}\n  method: get\n  operationId: get_82\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/inbound-trunk-numbers\n\
  \  method: get\n  operationId: get_68\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{participantExternalIdentifier}/targets/phone-extensions/{extensionNumber}/inbound-trunk-numbers\n  method: post\n  operationId: post_16\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenant.admin\n    - tenant.manager\n    - tenant.operator\n    - tenant.system-integrator\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{participantExternalIdentifier}\n\n# --- truncated at 32 KB (197 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/agentic-access/nfon-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nfon/refs/heads/main/agentic-access/nfon-agentic-access.yml
summary_line: 496 operations · 226 acting · 20 human-in-the-loop
tags:
- Company
- Telecom
- Cloud Telephony
- UCaaS
- CPaaS
- VoIP
- CTI
- Call History
- PBX
- Communications
- SIP
- Germany
---
