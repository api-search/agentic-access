---
acting_count: 989
action_class_counts:
  acting: 989
  connected: 942
api_specs:
- filename: webex-messaging-openapi.json
  format: json
  label: Webex Messaging
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-messaging-openapi.json
- filename: webex-meeting-openapi.json
  format: json
  label: Webex Meetings
  slug: meetings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-meeting-openapi.json
- filename: webex-admin-openapi.json
  format: json
  label: Webex Admin
  slug: admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-admin-openapi.json
- filename: webex-cloud-calling-openapi.json
  format: json
  label: Webex Cloud Calling
  slug: cloud-calling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-cloud-calling-openapi.json
- filename: webex-contact-center-openapi.json
  format: json
  label: Webex Contact Center
  slug: contact-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-contact-center-openapi.json
- filename: webex-device-openapi.json
  format: json
  label: Webex Devices
  slug: devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-device-openapi.json
- filename: webex-broadworks-openapi.json
  format: json
  label: Webex Broadworks Calling
  slug: broadworks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-broadworks-openapi.json
- filename: webex-ucm-openapi.json
  format: json
  label: Webex for UCM
  slug: ucm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-ucm-openapi.json
- filename: webex-wholesale-openapi.json
  format: json
  label: Webex Wholesale
  slug: wholesale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/openapi/webex-wholesale-openapi.json
consequence_counts:
  physical: 27
  read: 942
  safety-critical: 84
  write: 878
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 84
kind: agentic-access
layout: agentic-access
method: generated
name: Webex Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /admin/v1/api/person/add-identities/workspace-id/{workspaceId}/person-id/{personId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /meetings/controls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/contact-service-queue/fetch-by-dynamic-skills-and-skillProfile
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/contact-service-queue/fetch-by-userId-skillProfileId
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/overrides/bulk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /organization/{orgid}/overrides/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /organization/{orgid}/overrides/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/skill
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/skill-profile
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/skill-profile/bulk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /organization/{orgid}/skill-profile/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /organization/{orgid}/skill-profile/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/skill/bulk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/skill/populate-json-attr/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/skill/purge-inactive-entities
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /organization/{orgid}/skill/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /organization/{orgid}/skill/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /organization/{orgid}/user/bulk/update-dynamic-skill/{skillId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/user/fetch-by-skill-requirements
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /organization/{orgid}/user/{id}/reskill
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{orgid}/v2/contact-service-queue/fetch-by-grouped-assistant-skill
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /partner/organizations/partnerAdmin/{personId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /people/{personId}/features/voicemail/actions/resetPin/invoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/answer
operation_count: 1931
overview: 'Webex exposes 1931 API operations that an AI agent could call, of which 989 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 942 read, 878 write, 27 physical, and 84 safety-critical.


  84 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Webex
provider_slug: webex
slug: webex-agentic-access
source_filename: webex-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/webex-admin-openapi.json, openapi/webex-broadworks-openapi.json, openapi/webex-cloud-calling-openapi.json,\n  openapi/webex-contact-center-openapi.json, openapi/webex-device-openapi.json, openapi/webex-meeting-openapi.json,\n  openapi/webex-messaging-openapi.json, openapi/webex-ucm-openapi.json, openapi/webex-wholesale-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1931\n  by_action_class:\n    connected: 942\n    acting: 989\n  by_consequence:\n    read: 942\n    write: 878\n    safety-critical: 84\n    physical: 27\n  human_in_the_loop_required: 84\noperations:\n- path: /adminAudit/events\n  method: get\n  operationId: List Admin Audit Events\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adminAudit/eventCategories\n  method: get\n  operationId: List Admin Audit Event Categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations\n  method: get\n  operationId: listAuthorizationsForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations\n  method: delete\n  operationId: Delete authorization of org and client ID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorizations/{authorizationId}\n\
  \  method: delete\n  operationId: Delete authorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorizations/tokenExpiry\n  method: get\n  operationId: getTokenExpirationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classifications\n  method: get\n  operationId: List classifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataSources\n  method: post\n  operationId: Register a Data Source\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dataSources/\n  method: get\n  operationId: Retrieve All Data Sources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataSources/schemas\n  method: get\n  operationId: Retrieve Data Source Schemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataSources/schemas/{schemaId}\n  method: get\n  operationId: Retrieve Details of a Specific Data Source Schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataSources/{dataSourceId}\n  method: delete\n  operationId: Delete a Data Source\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dataSources/{dataSourceId}\n  method: get\n  operationId: Retrieve Data Source Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataSources/{dataSourceId}\n  method: put\n  operationId: Update a Data Source\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/organizations/{orgId}/v1/ArchivedUser/{useruuid}\n  method: get\n  operationId: getArchiveUser\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/organizations/{orgId}/actions/getDomainVerificationToken\n  method: post\n  operationId: Get Domain Verification Token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/organizations/{orgId}/actions/verifyDomain\n  method: post\n  operationId: Verify Domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/organizations/{orgId}/actions/claimDomain\n  method: post\n  operationId:\
  \ Claim Domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/organizations/{orgId}/actions/unverifyDomain\n  method: post\n  operationId: Unverify Domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/organizations/{orgId}/actions/unclaimDomain\n  method: post\n  operationId: Unclaim Domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /identity/organizations/{orgId}\n  method: get\n  operationId: Get an organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/organizations/{orgId}\n  method: patch\n  operationId: Update an organization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/organizations/{orgId}/users/{userId}/actions/generateOtp\n  method: post\n  operationId: Generate OTP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: List Events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}\n  method: get\n  operationId: Get Event Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: post\n  operationId: Create a Group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: get\n  operationId: List and Search Groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}\n  method: patch\n  operationId: Update a Group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}\n  method: get\n  operationId: Get Group Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}\n  method: delete\n  operationId: Delete a Group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/members\n\
  \  method: get\n  operationId: Get Group Members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /guests/token\n  method: post\n  operationId: Create a Guest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /guests/count\n  method: get\n  operationId: Get Guest Count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/messagingMetrics/dailyTotals\n  method: get\n  operationId: Historical Data related to Messaging\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/analytics/roomDeviceMetrics/dailyTotals\n  method: get\n  operationId: Historical Data related to Room Devices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/meetingsMetrics/aggregates\n  method: get\n  operationId: Historical Data related to Meetings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hybrid/clusters\n  method: get\n  operationId: List Hybrid Clusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hybrid/clusters/{hybridClusterId}\n  method: get\n  operationId: Get Hybrid Cluster Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /hybrid/connectors\n  method: get\n  operationId: List Hybrid Connectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hybrid/connectors/{connectorId}\n  method: get\n  operationId: Get Hybrid Connector Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licenses\n  method: get\n  operationId: List_Licenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licenses/{licenseId}\n  method: get\n  operationId: Get_License_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licenses/users\n  method: patch\n  operationId: Assign_Licenses_to_Users\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /livemonitoring/liveMeetingsByCountry\n  method: post\n  operationId: getLiveMeetingMetricsByCountry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meeting/qualities\n  method: get\n  operationId: getMeetingQualities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/organizations/{orgId}/contacts\n  method: post\n  operationId: Create a Contact\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/organizations/{orgId}/contacts/{contactId}\n  method: get\n  operationId: Get a Contact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/organizations/{orgId}/contacts/{contactId}\n  method: patch\n  operationId: Update a Contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/organizations/{orgId}/contacts/{contactId}\n  method: delete\n  operationId: Delete\
  \ a Contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/organizations/{orgId}/contacts/search\n  method: get\n  operationId: List Contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/organizations/{orgId}/contacts/bulk\n  method: post\n  operationId: Bulk Create or Update Contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/organizations/{orgId}/contacts/bulk/delete\n  method:\
  \ post\n  operationId: Bulk Delete Contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations\n  method: get\n  operationId: List Organizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{orgId}\n  method: get\n  operationId: Get Organization Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{orgId}\n  method: delete\n  operationId: Delete Organization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/organizations\n  method: get\n  operationId: Get all customers managed by a partner admin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/organizations/{orgId}/partnerAdmins\n  method: get\n  operationId: Get all partner admins assigned to a customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/organizations/{orgId}/partnerAdmin/{personId}/assign\n  method: post\n  operationId: Assign partner admin to a customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/organizations/{orgId}/partnerAdmin/{personId}/unassign\n  method: delete\n  operationId: Unassign partner admin from a customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/organizations/partnerAdmin/{personId}\n  method: delete\n  operationId: Revoke all partner admin roles for a given person ID\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /partner/reports\n  method: get\n \
  \ operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/reports\n  method: post\n  operationId: createAReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/reports/{reportId}\n  method: get\n  operationId: getReportDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/reports/{reportId}\n  method: delete\n  operationId: deleteAReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/reports/templates\n  method: get\n  operationId: listReportTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people\n  method: get\n  operationId: List People\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people\n  method: post\n  operationId: Create a Person\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{personId}\n  method: get\n  operationId: Get Person Details\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{personId}\n  method: put\n  operationId: Update a Person\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{personId}\n  method: delete\n  operationId: Delete a Person\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/me\n  method: get\n  operationId: Get My Own Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /recordingReport/accessSummary\n  method: get\n  operationId: List of Recording Audit Report Summaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordingReport/accessDetail\n  method: get\n  operationId: Get Recording Audit Report Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordingReport/meetingArchiveSummaries\n  method: get\n  operationId: List Meeting Archive Summaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordingReport/meetingArchives/{archiveId}\n  method: get\n  operationId: Get Meeting Archive Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordings\n  method: get\n  operationId: listRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/recordings\n  method: get\n  operationId: listRecordingsForAdminOrComplianceOfficer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/recordings/{recordingId}\n  method: delete\n  operationId: adminDeleteRecordingById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings/{recordingId}\n  method: get\n  operationId: getRecordByRecordId\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordings/{recordingId}\n  method: delete\n  operationId: deleteRecordingByRecordId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings/softDelete\n  method: post\n  operationId: bulkSoftDeleteRecordings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings/restore\n  method: post\n  operationId: bulkRestoreRecordings\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings/purge\n  method: post\n  operationId: bulkPurgeRecordings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings/{recordingId}/accessList\n  method: post\n  operationId: updateRecordingShareById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings/accessList\n  method: post\n\
  \  operationId: updateRecordingShareByLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/recordings\n  method: get\n  operationId: listGroupRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group/recordings/{recordingId}\n  method: get\n  operationId: getGroupRecordingById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/templates\n  method: get\n  operationId: List Report Templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports\n  method: post\n  operationId: createaReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{reportId}\n  method: get\n  operationId: getReportDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{reportId}\n  method: delete\n  operationId: deleteAReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resourceGroup/memberships\n  method: get\n  operationId: List Resource Group Memberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resourceGroup/memberships/v2\n  method: get\n  operationId: listResourceGroupMembershipsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resourceGroup/memberships/{resourceGroupMembershipId}\n  method: get\n  operationId: Get Resource Group Membership Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resourceGroup/memberships/{resourceGroupMembershipId}\n  method: put\n  operationId: Update\
  \ a Resource Group Membership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resourceGroups\n  method: get\n  operationId: List Resource Groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resourceGroups/{resourceGroupId}\n  method: get\n  operationId: Get Resource Group Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles\n  method: get\n  operationId: List Roles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /roles/{roleId}\n  method: get\n  operationId: Get Role Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/scim/{orgId}/v2/Bulk\n  method: post\n  operationId: User bulk API\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/scim/{orgId}/v2/Groups\n  method: post\n  operationId: Create a group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/scim/{orgId}/v2/Groups\n\
  \  method: get\n  operationId: Search groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/scim/{orgId}/v2/Groups/{groupId}\n  method: get\n  operationId: Get a group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/scim/{orgId}/v2/Groups/{groupId}\n  method: put\n  operationId: Update a group with PUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/scim/{orgId}/v2/Groups/{groupId}\n  method: patch\n  operationId: Update a group with PATCH\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/scim/{orgId}/v2/Groups/{groupId}\n  method: delete\n  operationId: Delete a group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/scim/{orgId}/v2/Groups/{groupId}/Members\n  method: get\n  operationId: Get Group Members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Schemas/SCIM2/Group\n  method: get\n  operationId: Get Group Schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Schemas/SCIM2/User\n  method: get\n  operationId: Get User Schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Schemas/SCIM2/{schemaId}\n  method: get\n  operationId: Get Schema using Group Schema ID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/scim/{orgId}/v2/Users\n  method: post\n  operationId: Create a user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/scim/{orgId}/v2/Users\n  method: get\n  operationId: Search users\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: opt\n\n# --- truncated at 32 KB (606 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/agentic-access/webex-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webex/refs/heads/main/agentic-access/webex-agentic-access.yml
summary_line: 1931 operations · 989 acting · 84 human-in-the-loop
tags:
- Calling
- Collaboration
- Communication
- Enterprise
- Messaging
- Video Conferencing
---
