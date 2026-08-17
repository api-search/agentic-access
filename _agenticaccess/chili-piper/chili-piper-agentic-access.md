---
acting_count: 54
action_class_counts:
  acting: 54
  connected: 19
api_specs:
- filename: chili-piper-availability-api-openapi.yml
  format: yaml
  label: Chili Piper Availability API
  slug: chili-piper-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-availability-api-openapi.yml
- filename: chili-piper-chat-api-openapi.yml
  format: yaml
  label: Chili Piper Chat API
  slug: chili-piper-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-chat-api-openapi.yml
- filename: chili-piper-concierge-api-openapi.yml
  format: yaml
  label: Chili Piper Concierge API
  slug: chili-piper-concierge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-concierge-api-openapi.yml
- filename: chili-piper-distribution-api-openapi.yml
  format: yaml
  label: Chili Piper Distribution API
  slug: chili-piper-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-distribution-api-openapi.yml
- filename: chili-piper-distro-api-openapi.yml
  format: yaml
  label: Chili Piper Distro API
  slug: chili-piper-distro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-distro-api-openapi.yml
- filename: chili-piper-handoff-api-openapi.yml
  format: yaml
  label: Chili Piper Handoff API
  slug: chili-piper-handoff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-handoff-api-openapi.yml
- filename: chili-piper-meeting-type-api-openapi.yml
  format: yaml
  label: Chili Piper Meeting Type API
  slug: chili-piper-meeting-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meeting-type-api-openapi.yml
- filename: chili-piper-meeting-type-reminder-api-openapi.yml
  format: yaml
  label: Chili Piper Meeting Type Reminder API
  slug: chili-piper-meeting-type-reminder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meeting-type-reminder-api-openapi.yml
- filename: chili-piper-meetings-api-openapi.yml
  format: yaml
  label: Chili Piper Meetings API
  slug: chili-piper-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-meetings-api-openapi.yml
- filename: chili-piper-rule-api-openapi.yml
  format: yaml
  label: Chili Piper Rule API
  slug: chili-piper-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-rule-api-openapi.yml
- filename: chili-piper-schedulinglinks-api-openapi.yml
  format: yaml
  label: Chili Piper Scheduling Links API
  slug: chili-piper-schedulinglinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-schedulinglinks-api-openapi.yml
- filename: chili-piper-team-api-openapi.yml
  format: yaml
  label: Chili Piper Team API
  slug: chili-piper-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-team-api-openapi.yml
- filename: chili-piper-tenant-api-openapi.yml
  format: yaml
  label: Chili Piper Tenant API
  slug: chili-piper-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-tenant-api-openapi.yml
- filename: chili-piper-user-api-openapi.yml
  format: yaml
  label: Chili Piper User API
  slug: chili-piper-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-user-api-openapi.yml
- filename: chili-piper-workspace-api-openapi.yml
  format: yaml
  label: Chili Piper Workspace API
  slug: chili-piper-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/openapi/chili-piper-workspace-api-openapi.yml
consequence_counts:
  physical: 4
  read: 19
  write: 50
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chili Piper Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/schedulingLinks/list-ownership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/schedulingLinks/ownership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/org/schedulingLinks/ownership/{linkId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/org/schedulingLinks/ownership/{linkId}
operation_count: 73
overview: 'Chili Piper exposes 73 API operations that an AI agent could call, of which 54 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 50 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chili Piper
provider_slug: chili-piper
slug: chili-piper-agentic-access
source_filename: chili-piper-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/chili-piper-availability-api-openapi.yml, openapi/chili-piper-chat-api-openapi.yml,\n  openapi/chili-piper-concierge-api-openapi.yml, openapi/chili-piper-distribution-api-openapi.yml,\n  openapi/chili-piper-distro-api-openapi.yml, openapi/chili-piper-handoff-api-openapi.yml, openapi/chili-piper-meeting-type-api-openapi.yml,\n  openapi/chili-piper-meeting-type-reminder-api-openapi.yml, openapi/chili-piper-meetings-api-openapi.yml,\n  openapi/chili-piper-rule-api-openapi.yml, openapi/chili-piper-schedulinglinks-api-openapi.yml,\n  openapi/chili-piper-team-api-openapi.yml, openapi/chili-piper-tenant-api-openapi.yml, openapi/chili-piper-user-api-openapi.yml,\n  openapi/chili-piper-workspace-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment.\
  \ See research/curity/agentic-governance/.\nsummary:\n  operations: 73\n  by_action_class:\n    acting: 54\n    connected: 19\n  by_consequence:\n    write: 50\n    read: 19\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/org/availability/slots\n  method: post\n  operationId: availabilitySlots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/chat/logs\n  method: get\n  operationId: chatLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/concierge/routers/concierge/list\n  method: post\n  operationId: conciergeListRouters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/concierge/logs\n  method: post\n  operationId: conciergeLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/concierge/routers/concierge\n  method: post\n  operationId: conciergeRouterCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/concierge/routers/concierge/{routerId}\n  method: get\n  operationId:\
  \ conciergeRouterGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/concierge/routers/concierge/{routerId}\n  method: put\n  operationId: conciergeRouterUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/concierge/routers/concierge/{routerId}\n  method: delete\n  operationId: conciergeRouterDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/distribution\n  method: post\n  operationId:\
  \ distributionCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/org/distribution/list\n  method: put\n  operationId: distributionListPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/distribution/workspace-settings\n  method: get\n  operationId: distributionWorkspaceSettingsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/distro/logs\n  method: post\n  operationId: distroLogs\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/distro/logs/{logId}\n  method: get\n  operationId: distroLogGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/distro/routers/list\n  method: post\n  operationId: distroListRouters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/distro/routers/{routerId}\n  method: get\n  operationId: distroRouterGet\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/distro/routers/{routerId}\n  method: put\n  operationId: distroRouterUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/distro/routers/{routerId}\n  method: delete\n  operationId: distroRouterDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/distro/routers\n  method: post\n  operationId: distroRouterCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/distro/routers/{routerId}/activate\n  method: post\n  operationId: distroRouterActivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/distro/routers/{routerId}/deactivate\n  method: post\n  operationId: distroRouterDeactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/handoff/routers/handoff/list\n \
  \ method: get\n  operationId: handoffRouterList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/handoff/routers/handoff/{routerId}\n  method: get\n  operationId: handoffRouterGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/handoff/routers/handoff/{routerId}\n  method: put\n  operationId: handoffRouterUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/handoff/routers/handoff/{routerId}\n  method: delete\n  operationId: handoffRouterDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/handoff/routers/handoff\n  method: post\n  operationId: handoffRouterCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meeting-types\n  method: post\n  operationId: meetingTypeCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meeting-types/list\n  method: get\n  operationId:\
  \ meetingTypeList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/meeting-types/{meetingTypeId}\n  method: get\n  operationId: meetingTypeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/meeting-types/{meetingTypeId}\n  method: put\n  operationId: meetingTypeUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meeting-types/{meetingTypeId}\n  method: delete\n  operationId: meetingTypeDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meeting-types/{meetingTypeId}/reminders/{reminderId}\n  method: put\n  operationId: meetingTypeAttachReminder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meeting-types/{meetingTypeId}/reminders/{reminderId}\n  method: delete\n  operationId: meetingTypeDetachReminder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meeting-type-reminders/list\n\
  \  method: get\n  operationId: meetingTypeReminderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/meeting-type-reminders\n  method: post\n  operationId: meetingTypeReminderCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meeting-type-reminders/{reminderId}\n  method: put\n  operationId: meetingTypeReminderUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meeting-type-reminders/{reminderId}\n\
  \  method: delete\n  operationId: meetingTypeReminderDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/org/meetings/meetings\n  method: put\n  operationId: meetingListPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meetings/get/{meetingId}\n  method: get\n  operationId: meetingGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/org/meetings/meetings/export\n  method: put\n  operationId: meetingExportV2Put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/meetings/cancel/{meetingId}\n  method: get\n  operationId: meetingCancel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/rule/list\n  method: get\n  operationId: ruleList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/rule\n  method: post\n  operationId: ruleCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/list-personal/{userId}\n  method: get\n  operationId: schedulingLinkListPersonal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/schedulingLinks/list-round-robin\n  method: post\n  operationId: schedulingLinkListRoundRobin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/list-admin-one-on-one\n  method: post\n  operationId: schedulingLinkListAdminOneOnOne\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/list-group\n  method: post\n  operationId: schedulingLinkListGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/list-ownership\n  method: post\n  operationId: schedulingLinkListOwnership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/round-robin\n  method: post\n  operationId: schedulingLinkCreateRoundRobin\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/round-robin/{linkId}\n  method: put\n  operationId: schedulingLinkUpdateRoundRobin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/round-robin/{linkId}\n  method: delete\n  operationId: schedulingLinkDeleteRoundRobin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/admin-one-on-one\n  method: post\n  operationId: schedulingLinkCreateAdminOneOnOne\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/admin-one-on-one/{linkId}\n  method: put\n  operationId: schedulingLinkUpdateAdminOneOnOne\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/admin-one-on-one/{linkId}\n  method: delete\n  operationId: schedulingLinkDeleteAdminOneOnOne\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/group\n  method: post\n  operationId: schedulingLinkCreateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/group/{linkId}\n  method: put\n  operationId: schedulingLinkUpdateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/org/schedulingLinks/group/{linkId}\n  method: delete\n  operationId: schedulingLinkDeleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/ownership\n  method: post\n  operationId: schedulingLinkCreateOwnership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/ownership/{linkId}\n  method: put\n  operationId: schedulingLinkUpdateOwnership\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/schedulingLinks/ownership/{linkId}\n  method: delete\n  operationId: schedulingLinkDeleteOwnership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/org/team/create\n  method: post\n  operationId: teamCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/team/users/add\n  method: post\n  operationId: teamAddUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/org/team\n  method: put\n  operationId: teamListPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/team/users/remove\n  method: post\n  operationId: teamRemoveUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/org/team/{teamId}\n  method: delete\n  operationId: teamDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/tenant/get\n  method: get\n  operationId: tenantGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/user/find\n  method: get\n  operationId: userFind\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/user/read/{userId}\n  method: get\n  operationId: userRead\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/user/find-by-id\n  method: post\n  operationId: userFindByIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/user/licenses\n  method: post\n  operationId: userUpdateLicenses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/workspace\n  method: get\n  operationId: workspaceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/org/workspace/users\n  method: get\n  operationId: workspaceListUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/workspace/users/add\n  method: post\n  operationId: workspaceAddUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/workspace/users/remove\n  method: post\n  operationId: workspaceRemoveUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chili-piper/refs/heads/main/agentic-access/chili-piper-agentic-access.yml
summary_line: 73 operations · 54 acting
tags:
- Scheduling
- Lead Routing
- Meetings
- Sales
- Marketing
- CRM
- Demand Conversion
- Appointment Booking
- Revenue Operations
- Calendar
- Agents
- MCP
---
