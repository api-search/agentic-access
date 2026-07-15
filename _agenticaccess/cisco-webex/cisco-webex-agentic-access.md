---
acting_count: 50
action_class_counts:
  acting: 50
  connected: 42
api_specs:
- filename: cisco-webex-meetings-openapi.yml
  format: yaml
  label: Webex Meetings API
  slug: webex-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-meetings-openapi.yml
- filename: cisco-webex-messaging-openapi.yml
  format: yaml
  label: Webex Messaging API
  slug: webex-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-messaging-openapi.yml
- filename: cisco-webex-people-openapi.yml
  format: yaml
  label: Webex People API
  slug: webex-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-people-openapi.yml
- filename: cisco-webex-teams-openapi.yml
  format: yaml
  label: Webex Teams API
  slug: webex-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-teams-openapi.yml
- filename: cisco-webex-rooms-openapi.yml
  format: yaml
  label: Webex Rooms API
  slug: webex-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-rooms-openapi.yml
- filename: cisco-webex-webhooks-openapi.yml
  format: yaml
  label: Webex Webhooks API
  slug: webex-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-webhooks-openapi.yml
- filename: cisco-webex-devices-openapi.yml
  format: yaml
  label: Webex Devices API
  slug: webex-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-devices-openapi.yml
- filename: cisco-webex-memberships-openapi.yml
  format: yaml
  label: Webex Memberships API
  slug: webex-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-memberships-openapi.yml
- filename: cisco-webex-team-memberships-openapi.yml
  format: yaml
  label: Webex Team Memberships API
  slug: webex-team-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-team-memberships-openapi.yml
- filename: cisco-webex-events-openapi.yml
  format: yaml
  label: Webex Events API
  slug: webex-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-events-openapi.yml
- filename: cisco-webex-recordings-openapi.yml
  format: yaml
  label: Webex Recordings API
  slug: webex-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-recordings-openapi.yml
- filename: cisco-webex-call-controls-openapi.yml
  format: yaml
  label: Webex Call Controls API
  slug: webex-call-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-call-controls-openapi.yml
- filename: cisco-webex-attachment-actions-openapi.yml
  format: yaml
  label: Webex Attachment Actions API
  slug: webex-attachment-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-attachment-actions-openapi.yml
- filename: cisco-webex-organizations-openapi.yml
  format: yaml
  label: Webex Organizations API
  slug: webex-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-organizations-openapi.yml
- filename: cisco-webex-licenses-openapi.yml
  format: yaml
  label: Webex Licenses API
  slug: webex-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-licenses-openapi.yml
- filename: cisco-webex-roles-openapi.yml
  format: yaml
  label: Webex Roles API
  slug: webex-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-roles-openapi.yml
- filename: cisco-webex-workspaces-openapi.yml
  format: yaml
  label: Webex Workspaces API
  slug: webex-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-workspaces-openapi.yml
- filename: cisco-webex-admin-audit-events-openapi.yml
  format: yaml
  label: Webex Admin Audit Events API
  slug: webex-admin-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-admin-audit-events-openapi.yml
- filename: cisco-webex-converged-recordings-openapi.yml
  format: yaml
  label: Webex Converged Recordings API
  slug: webex-converged-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/openapi/cisco-webex-converged-recordings-openapi.yml
consequence_counts:
  physical: 6
  read: 42
  safety-critical: 9
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 9
kind: agentic-access
layout: agentic-access
method: generated
name: Cisco Webex Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/answer
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/dial
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/hangup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/hold
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/park
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/reject
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/resume
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/retrieve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /telephony/calls/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /memberships/{membershipId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /memberships/{membershipId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /team/memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /team/memberships/{membershipId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /team/memberships/{membershipId}
operation_count: 92
overview: 'Cisco Webex exposes 92 API operations that an AI agent could call, of which 50 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 42 read, 35 write, 6 physical, and 9 safety-critical.


  9 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cisco Webex
provider_slug: cisco-webex
slug: cisco-webex-agentic-access
source_filename: cisco-webex-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cisco-webex-admin-audit-events-openapi.yml, openapi/cisco-webex-attachment-actions-openapi.yml,\n  openapi/cisco-webex-call-controls-openapi.yml, openapi/cisco-webex-converged-recordings-openapi.yml,\n  openapi/cisco-webex-devices-openapi.yml, openapi/cisco-webex-events-openapi.yml, openapi/cisco-webex-licenses-openapi.yml,\n  openapi/cisco-webex-meetings-openapi.yml, openapi/cisco-webex-memberships-openapi.yml, openapi/cisco-webex-messaging-openapi.yml,\n  openapi/cisco-webex-organizations-openapi.yml, openapi/cisco-webex-people-openapi.yml, openapi/cisco-webex-recordings-openapi.yml,\n  openapi/cisco-webex-roles-openapi.yml, openapi/cisco-webex-rooms-openapi.yml, openapi/cisco-webex-team-memberships-openapi.yml,\n  openapi/cisco-webex-teams-openapi.yml, openapi/cisco-webex-webhooks-openapi.yml, openapi/cisco-webex-workspaces-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically\
  \ from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 92\n  by_action_class:\n    connected: 42\n    acting: 50\n  by_consequence:\n    read: 42\n    write: 35\n    safety-critical: 9\n    physical: 6\n  human_in_the_loop_required: 9\noperations:\n- path: /adminAudit/events\n  method: get\n  operationId: listAdminAuditEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adminAudit/eventCategories\n  method: get\n  operationId: listAdminAuditEventCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachment/actions\n  method: post\n  operationId: createAttachmentAction\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachment/actions/{id}\n  method: get\n  operationId: getAttachmentActionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /telephony/calls/dial\n  method: post\n  operationId: dial\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /telephony/calls/answer\n  method: post\n  operationId: answer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /telephony/calls/reject\n  method: post\n  operationId: reject\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /telephony/calls/hangup\n  method: post\n  operationId: hangup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /telephony/calls/hold\n  method: post\n  operationId: hold\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /telephony/calls/resume\n  method: post\n  operationId: resume\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /telephony/calls/transfer\n  method: post\n  operationId: transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n     \
  \ exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /telephony/calls/park\n  method: post\n  operationId: park\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /telephony/calls/retrieve\n  method: post\n  operationId: retrieve\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /telephony/calls\n  method: get\n  operationId: listCalls\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /telephony/calls/{callId}\n  method: get\n  operationId: getCallDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convergedRecordings\n  method: get\n  operationId: listConvergedRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convergedRecordings/{recordingId}\n  method: get\n  operationId: getConvergedRecordingDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convergedRecordings/{recordingId}\n  method: delete\n  operationId: deleteConvergedRecording\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: post\n  operationId: createDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}\n  method: get\n  operationId: getDeviceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceId}\n\
  \  method: put\n  operationId: updateDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}\n  method: delete\n  operationId: deleteDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}\n  method: get\n  operationId: getEventDetails\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licenses\n  method: get\n  operationId: listLicenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licenses/{licenseId}\n  method: get\n  operationId: getLicenseDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licenses/users\n  method: patch\n  operationId: assignLicensesToUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings\n  method: get\n  operationId: listMeetings\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meetings\n  method: post\n  operationId: createMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/{meetingId}\n  method: get\n  operationId: getMeetingDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meetings/{meetingId}\n  method: put\n  operationId: updateMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /meetings/{meetingId}\n  method: delete\n  operationId: deleteMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/{meetingId}/registrants\n  method: get\n  operationId: listMeetingRegistrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meetings/{meetingId}/registrants/approve\n  method: post\n  operationId: approveMeetingRegistrants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /meetings/{meetingId}/registrants/reject\n  method: post\n  operationId: rejectMeetingRegistrants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/{meetingId}/registrants/cancel\n  method: post\n  operationId: cancelMeetingRegistrants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/{meetingId}/registrants/bulkInsert\n  method: post\n  operationId: batchRegisterMeetingRegistrants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meetings/{meetingId}/registrants/bulkDelete\n  method: post\n  operationId: batchDeleteMeetingRegistrants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /memberships\n  method: get\n  operationId: listMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memberships\n  method: post\n  operationId: createMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /memberships/{membershipId}\n  method: get\n  operationId: getMembershipDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memberships/{membershipId}\n  method: put\n  operationId: updateMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /memberships/{membershipId}\n  method: delete\n  operationId: deleteMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/direct\n  method: get\n  operationId: listDirectMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /messages/{messageId}\n  method: get\n  operationId: getMessageDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{messageId}\n  method: put\n  operationId: editMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{messageId}\n  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations\n  method: get\n  operationId: listOrganizations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{orgId}\n  method: get\n  operationId: getOrganizationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{orgId}\n  method: delete\n  operationId: deleteOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people\n  method: get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people\n  method: post\n  operationId: createPerson\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/me\n  method: get\n  operationId: getMyOwnDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{personId}\n  method: get\n  operationId: getPersonDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{personId}\n  method: put\n  operationId: updatePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /people/{personId}\n  method: delete\n  operationId: deletePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings\n  method: get\n  operationId: listRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordings/{recordingId}\n  method: get\n  operationId: getRecordingDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordings/{recordingId}\n  method: delete\n  operationId: deleteRecording\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/recordings\n  method: get\n  operationId: listAdminRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/recordings/{recordingId}\n  method: delete\n  operationId: deleteAdminRecording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /roles/{roleId}\n  method: get\n  operationId: getRoleDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms\n  method: get\n  operationId: listRooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms\n  method: post\n  operationId: createRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}\n  method: get\n  operationId: getRoomDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/{roomId}\n\
  \  method: put\n  operationId: updateRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}\n  method: delete\n  operationId: deleteRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/meetingInfo\n  method: get\n  operationId: getRoomMeetingDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/memberships\n  method: get\n  operationId: listTeamMemberships\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/memberships\n  method: post\n  operationId: createTeamMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/memberships/{membershipId}\n  method: get\n  operationId: getTeamMembershipDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/memberships/{membershipId}\n  method: put\n  operationId: updateTeamMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/memberships/{membershipId}\n  method: delete\n  operationId: deleteTeamMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: post\n  operationId: createTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{teamId}\n  method: get\n  operationId: getTeamDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{teamId}\n  method: put\n  operationId: updateTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{teamId}\n  method: delete\n  operationId: deleteTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: get\n  operationId: getWebhookDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhookId}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}\n  method: get\n  operationId: getWorkspaceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}\n  method: put\n  operationId: updateWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}\n  method: delete\n  operationId: deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/agentic-access/cisco-webex-agentic-access.yml
summary_line: 92 operations · 50 acting · 9 human-in-the-loop
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
---
