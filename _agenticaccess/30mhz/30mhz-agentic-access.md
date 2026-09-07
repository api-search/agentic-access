---
acting_count: 319
action_class_counts:
  acting: 319
  connected: 239
api_specs:
- filename: 30mhz-zensie-openapi.json
  format: json
  label: ZENSIE API
  slug: zensie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/30mhz/refs/heads/main/openapi/30mhz-zensie-openapi.json
consequence_counts:
  physical: 19
  read: 239
  safety-critical: 3
  write: 297
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: 30Mhz Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-check/copy/{checkId}/organization/{destinationOrganizationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /user/api-key
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /user/{email}/api-key
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agent/message-stream
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-update/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-update/{checkId}/new-organization/{newOrganizationId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /check-update/{checkId}/new-owner/{newOwner}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /dashboard-update/group/{groupId}/dashboard/{dashboardId}/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /dashboard-update/organization/{organizationId}/dashboard/{dashboardId}/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /import-check-update/{checkId}/collection/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice-update/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /invoice/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order-update/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /order/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{orderId}/invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization-update/{organizationId}/user/{email}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /organization/{organizationId}/user/{email}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /organization/{organizationId}/user/{email}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /quote/{quoteId}/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /util/contact
operation_count: 558
overview: '30MHz exposes 558 API operations that an AI agent could call, of which 319 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 239 read, 297 write, 19 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 30MHz
provider_slug: 30mhz
slug: 30mhz-agentic-access
source_filename: 30mhz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: generated\nsource: openapi/30mhz-zensie-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 558\n  by_action_class:\n    connected: 239\n    acting: 319\n  by_consequence:\n    read: 239\n    write: 297\n    physical: 19\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /admin/health/api-build-version\n  method: get\n  operationId: getApiBuildVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/health/auth0\n  method: get\n  operationId: getAuth0Health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /admin/health/dynamodb\n  method: get\n  operationId: getDynamoDbHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/health/elasticsearch\n  method: get\n  operationId: getElasticsearchHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/health/scheduler\n  method: get\n  operationId: getSchedulerHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/notification-follow/user/{email}\n  method: delete\n  operationId: deleteAllNotificationFollowsOfUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/conversation/{conversationId}/message\n  method: get\n  operationId: getConversationMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/message-stream\n  method: post\n  operationId: sendMessageStream\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assembly\n  method: post\n  operationId: createAssembly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assembly/{serialNumber}\n  method: get\n  operationId: getAssembly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assembly/{serialNumber}\n  method: delete\n  operationId: deleteAssembly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assembly/xbee/{xbee}\n  method: get\n  operationId: getAssemblyByXbee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assembly/{serialNumber}/history\n  method: get\n\
  \  operationId: getAssemblyHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assembly/xbee/{xbee}/history\n  method: get\n  operationId: getAssemblyHistoryByXbee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assembly-update/{serialNumber}\n  method: post\n  operationId: updateAssembly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/device/jwks\n  method: get\n  operationId: getDevicePublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /authorization/license/oauth/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/role-assignment/assignee/{assignee}/role/{role}/license/{licenseId}\n  method: post\n  operationId: assignRoleOnLicense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/role-assignment/assignee/{assignee}/role/{role}/license/{licenseId}\n  method: delete\n  operationId: unassignRoleOnLicense\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/role-assignment/assignee/{assignee}/role/{role}/organization/{organizationId}\n  method: post\n  operationId: assignRoleOnOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/role-assignment/assignee/{assignee}/role/{role}/organization/{organizationId}\n  method: delete\n  operationId: unassignRoleOnOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/role-assignment/assignee/{assignee}/role/{role}/device/{deviceId}\n  method: post\n  operationId: assignRoleOnDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/role-assignment/assignee/{assignee}/role/{role}/device/{deviceId}\n  method: delete\n  operationId: unassignRoleOnDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/role-assignment/assignee/{assignee}/role/{role}/organization/{organizationId}/site/{siteId}\n\
  \  method: post\n  operationId: assignRoleOnSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/role-assignment/assignee/{assignee}/role/{role}/organization/{organizationId}/site/{siteId}\n  method: delete\n  operationId: unassignRoleOnSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/check/device/{deviceId}\n  method: get\n  operationId: checkUserAuthorizationOnDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /authorization/check/organization/{organizationId}\n  method: get\n  operationId: checkUserAuthorizationOnOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/check/organization/{organizationId}/site/{siteId}\n  method: get\n  operationId: checkUserAuthorizationOnSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/device/{deviceId}/access-token\n  method: get\n  operationId: getDeviceAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/role-assignment\n  method: get\n  operationId: getRoleAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/role-assignment/assignee/{assignee}/organization/{organizationId}\n  method: get\n  operationId: getRoleAssignmentsOfUserOnOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/role-assignment/assignee/{assignee}/license/{licenseId}\n  method: get\n  operationId: getRoleAssignmentsOfUserUnderLicense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/role-assignment/organization/{organizationId}\n  method: get\n  operationId: getRoleAssignmentsOnOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/scopes\n  method: get\n  operationId:\
  \ getScopesAndClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-history-details/{billingHistoryDetailsId}\n  method: get\n  operationId: getBillingHistoryDetailsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-history-details/organization/{organizationId}/year/{year}/month/{month}\n  method: get\n  operationId: getBillingHistoryDetailsByOrganizationIdAndMonth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-history-details/organization/{organizationId}/year/{year}/month/{month}/json/{jsonCheck}\n  method: get\n  operationId: getBillingHistoryDetailsChecksJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-history-details/organization/{organizationId}/year/{year}/month/{month}/mother\n  method: get\n  operationId: getBillingHistoryDetailsMothersByOrgIdAndMonth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-history-details-update/organization/{organizationId}/year/{year}/month/{month}/mother/{motherId}\n  method: post\n  operationId: updateBillingHistoryByMother\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-history-details-update/{billingHistoryDetailsId}\n  method: post\n  operationId: updateBillingHistoryDetails\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-history/organization/{organizationId}/year/{year}/month/{month}\n  method: get\n  operationId: getBillingHistoryByOrganizationIdAndMonth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-history/organization/{organizationId}/year/{year}/month/{month}\n  method: delete\n  operationId: deleteBillingHistoryByOrganizationAndMonth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-history/organization/{organizationId}\n\
  \  method: get\n  operationId: getBillingHistoryByOrganizationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-history/organization/{organizationId}/forecast\n  method: post\n  operationId: getBillingHistoryForecastForCurrentMonth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-history/all-organizations/year/{year}/month/{month}\n  method: get\n  operationId: getBillingHistoryOrganisationsByMonth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-history/all-organizations\n  method: get\n  operationId: getBillingHistoryOrganisationsCurrentMonth\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-history/all-organizations\n  method: post\n  operationId: createSqsBillingHistoryRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-history\n  method: post\n  operationId: createSqsBillingHistoryRequestForOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-history-update/organization/{organizationId}/year/{year}/month/{month}\n\
  \  method: post\n  operationId: updateBillingHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chart/scatterplot\n  method: post\n  operationId: getScatterplot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chart/cultivation-target\n  method: post\n  operationId: getCultivationTargetSeriesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /check/{checkId}\n  method: get\n  operationId: getCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check/{checkId}\n  method: delete\n  operationId: removeCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check/sensor/default\n  method: get\n  operationId: getDefaultSensorCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check/organization/{organizationId}/clone/check/{checkId}\n  method: post\n  operationId: cloneCheck\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check/organization/{organizationId}\n  method: get\n  operationId: getOrganizationChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check/organization/{organizationId}\n  method: post\n  operationId: createWebcheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check/gateway-cluster/{gatewayClusterId}\n  method: get\n  operationId: getGatewayClusterSensors\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check/gateway/{gatewayId}\n  method: get\n  operationId: getGatewaySensors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check/delete-batch\n  method: post\n  operationId: removeChecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check/default\n  method: get\n  operationId: getDefaultCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-update/{checkId}/new-organization/{newOrganizationId}\n  method: post\n  operationId:\
  \ transferCheckOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-update/{checkId}/new-owner/{newOwner}\n  method: post\n  operationId: transferCheckOwnership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-update/transfer\n  method: post\n  operationId: transferChecks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-update/{checkId}\n  method: post\n  operationId: updateCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-update\n  method: post\n  operationId: updateChecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comment/{commentId}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comment/{commentId}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comment\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comment/reply/{commentId}\n  method: post\n  operationId: createReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comment/interval\n  method: get\n  operationId: getCommentsByInterval\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comment/timeinterval\n  method: get\n  operationId: getCommentsByTimeInterval\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comment/feed/group/{groupId}\n  method: get\n  operationId: getCommentsFeedForGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comment/feed/organization/{organizationId}\n  method: get\n  operationId: getCommentsFeedForOrganization\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comment/interval/{interval}\n  method: post\n  operationId: getCommentsForInterval\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comment/from/{startDate}/until/{endDate}\n  method: post\n  operationId: getCommentsForTimeInterval\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comment/paginated-feed/group/{groupId}\n  method: get\n  operationId: getPaginatedCommentsFeedForGroup\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comment/paginated-feed/organization/{organizationId}\n  method: get\n  operationId: getPaginatedCommentsFeedForOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comment/search\n  method: post\n  operationId: searchForComments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comment-update/{commentId}\n  method: post\n  operationId: updateComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comment-update/reply/{commentId}\n  method: post\n  operationId: commentReplyUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company-details/{companyDetailsId}\n  method: delete\n  operationId: deleteCompanyDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company-details/organization/{organizationId}\n  method: get\n  operationId: getCompanyDetailsByOrganizationId\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company-details/organization/{organizationId}\n  method: post\n  operationId: createCompanyDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company-details-update/{companyDetailsId}\n  method: post\n  operationId: updateCompanyDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crop\n  method: get\n  operationId: getPublicCrops\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crop\n  method: post\n  operationId: createCrop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crop/{cropId}\n  method: get\n  operationId: getCropById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crop/{cropId}\n  method: put\n  operationId: putCrop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crop/{cropId}\n\
  \  method: delete\n  operationId: deleteCrop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crop/{cropId}\n  method: patch\n  operationId: patchCrop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crop/organization/{organizationId}\n  method: get\n  operationId: getCropsForOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currency-rates\n  method: post\n  operationId: addCurrencyRates\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /currency\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currency\n  method: post\n  operationId: createCurrency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /currency/{currencyId}\n  method: delete\n  operationId: deleteCurrency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration/{registrationId}/activate\n  method: get\n  operationId: activateRegistration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registration/{registrationId}\n  method: delete\n  operationId: removeRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration\n  method: post\n  operationId: createRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/organization/{organizationId}\n  method: get\n  operationId: getDashboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/organization/{organizationId}\n  method: post\n  operationId: createDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/clone/{dashboardId}/group/{groupId}\n  method: post\n  operationId: cloneDashboardToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/organization/{organizationId}/diagnostics\n  method: post\n  operationId: createDiagnosticsDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/group/{groupId}\n  method: get\n  operationId: getDashboardsInGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/group/{groupId}\n  method: post\n  operationId: createGroupDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: n\n\n# --- truncated at 32 KB (167 KB total)\
  \ ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/30mhz/refs/heads/main/agentic-access/30mhz-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/30mhz/refs/heads/main/agentic-access/30mhz-agentic-access.yml
summary_line: 558 operations · 319 acting · 3 human-in-the-loop
tags:
- Horticulture
- Agriculture
- AgTech
- Sensors
- Internet of Things
- Greenhouse
- Climate Monitoring
- Time Series Data
- Data Platform
- Netherlands
---
