---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 9
api_specs:
- filename: microsoft-teams-graph-api.yaml
  format: yaml
  label: Microsoft Graph Teams API
  slug: microsoft-graph-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-graph-api.yaml
- filename: microsoft-teams-asyncapi.yaml
  format: yaml
  label: Microsoft Teams Bot Framework API
  slug: microsoft-teams-bot-framework-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/asyncapi/microsoft-teams-asyncapi.yaml
consequence_counts:
  physical: 4
  read: 9
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Teams Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /communications/calls/{call-id}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /teams/{team-id}/channels/{channel-id}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /teams/{team-id}/members/{membership-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /teams/{team-id}/members/{membership-id}
operation_count: 24
overview: 'Microsoft Teams exposes 24 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 11 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Teams
provider_slug: microsoft-teams
slug: microsoft-teams-agentic-access
source_filename: microsoft-teams-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-teams-graph-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 9\n    acting: 15\n  by_consequence:\n    read: 9\n    write: 11\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /me/joinedTeams\n  method: get\n  operationId: listJoinedTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams\n  method: post\n  operationId: createTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}\n  method: patch\n  operationId: updateTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n\
  \    - Team.ReadBasic.All\n- path: /teams/{team-id}\n  method: delete\n  operationId: deleteTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/archive\n  method: post\n  operationId: archiveTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/channels\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/channels\n  method: post\n  operationId: createChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/channels/{channel-id}/messages\n  method: get\n  operationId: listChannelMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n\
  - path: /teams/{team-id}/channels/{channel-id}/messages\n  method: post\n  operationId: sendChannelMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/channels/{channel-id}/tabs\n  method: get\n  operationId: listChannelTabs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/installedApps\n  method: get\n  operationId: listInstalledApps\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/members\n  method: get\n  operationId: listTeamMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/members\n  method: post\n  operationId: addTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/members/{membership-id}\n\
  \  method: delete\n  operationId: removeTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /teams/{team-id}/members/{membership-id}\n  method: patch\n  operationId: updateTeamMember\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n-\
  \ path: /communications/onlineMeetings\n  method: post\n  operationId: createOnlineMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /communications/onlineMeetings/{meeting-id}\n  method: get\n  operationId: getOnlineMeeting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /communications/calls\n  method: post\n  operationId: createCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /communications/calls/{call-id}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /communications/calls/{call-id}\n  method: delete\n  operationId: hangUpCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n\
  - path: /communications/calls/{call-id}/answer\n  method: post\n  operationId: answerCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /communications/calls/{call-id}/reject\n  method: post\n  operationId: rejectCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n- path: /communications/calls/{call-id}/transfer\n  method: post\n  operationId: transferCall\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Channel.ReadBasic.All\n    - ChatMessage.Read\n    - Team.ReadBasic.All\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/agentic-access/microsoft-teams-agentic-access.yml
summary_line: 24 operations · 15 acting
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
---
