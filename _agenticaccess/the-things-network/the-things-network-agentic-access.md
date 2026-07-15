---
acting_count: 174
action_class_counts:
  acting: 174
  connected: 155
api_specs:
- filename: the-things-stack-identity-server-openapi.yml
  format: yaml
  label: The Things Stack Identity Server
  slug: the-things-stack-identity-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-identity-server-openapi.yml
- filename: the-things-stack-application-server-openapi.yml
  format: yaml
  label: The Things Stack Application Server
  slug: the-things-stack-application-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-application-server-openapi.yml
- filename: the-things-stack-network-server-openapi.yml
  format: yaml
  label: The Things Stack Network Server
  slug: the-things-stack-network-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-network-server-openapi.yml
- filename: the-things-stack-gateway-server-openapi.yml
  format: yaml
  label: The Things Stack Gateway Server
  slug: the-things-stack-gateway-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-gateway-server-openapi.yml
- filename: the-things-stack-join-server-openapi.yml
  format: yaml
  label: The Things Stack Join Server
  slug: the-things-stack-join-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-join-server-openapi.yml
- filename: the-things-stack-end-device-registry-openapi.yml
  format: yaml
  label: The Things Stack End Device Registry
  slug: the-things-stack-end-device-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-end-device-registry-openapi.yml
- filename: the-things-stack-integrations-openapi.yml
  format: yaml
  label: The Things Stack Integrations
  slug: the-things-stack-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-integrations-openapi.yml
- filename: the-things-stack-packet-broker-agent-openapi.yml
  format: yaml
  label: The Things Stack Packet Broker Agent
  slug: the-things-stack-packet-broker-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-packet-broker-agent-openapi.yml
- filename: the-things-stack-events-openapi.yml
  format: yaml
  label: The Things Stack Events
  slug: the-things-stack-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/openapi/the-things-stack-events-openapi.yml
consequence_counts:
  physical: 19
  read: 155
  safety-critical: 3
  write: 152
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: The Things Network Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /invitations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /ns/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /users/{user_ids.user_id}/sessions/{session_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /as/applications/{application_ids.application_id}/devices/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /as/applications/{application_ids.application_id}/devices/{device_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /as/applications/{end_device.ids.application_ids.application_id}/devices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /as/applications/{end_device.ids.application_ids.application_id}/devices/{end_device.ids.device_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edcs/applications/{application_ids.application_id}/authorize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /edcs/applications/{application_id}/authorize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gcls/claim
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invitations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /js/applications/{application_ids.application_id}/devices/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /js/applications/{application_ids.application_id}/devices/{device_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /js/applications/{application_ids.application_id}/provision-devices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /js/applications/{end_device.ids.application_ids.application_id}/devices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /js/applications/{end_device.ids.application_ids.application_id}/devices/{end_device.ids.device_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /ns/applications/{application_ids.application_id}/devices/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ns/applications/{application_ids.application_id}/devices/mac_settings_profile/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /ns/applications/{application_ids.application_id}/devices/{device_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ns/applications/{end_device.ids.application_ids.application_id}/devices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ns/applications/{end_device.ids.application_ids.application_id}/devices/{end_device.ids.device_id}
operation_count: 329
overview: 'The Things Network / The Things Stack exposes 329 API operations that an AI agent could call, of which 174 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 155 read, 152 write, 19 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Things Network / The Things Stack
provider_slug: the-things-network
slug: the-things-network-agentic-access
source_filename: the-things-network-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/the-things-stack-application-server-openapi.yml, openapi/the-things-stack-end-device-registry-openapi.yml,\n  openapi/the-things-stack-events-openapi.yml, openapi/the-things-stack-gateway-server-openapi.yml,\n  openapi/the-things-stack-identity-server-openapi.yml, openapi/the-things-stack-integrations-openapi.yml,\n  openapi/the-things-stack-join-server-openapi.yml, openapi/the-things-stack-network-server-openapi.yml,\n  openapi/the-things-stack-packet-broker-agent-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 329\n  by_action_class:\n    connected: 155\n    acting: 174\n  by_consequence:\n    read: 155\n    write: 152\n    physical: 19\n    safety-critical: 3\n  human_in_the_loop_required:\
  \ 3\noperations:\n- path: /applications\n  method: get\n  operationId: ApplicationRegistry_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application.ids.application_id}\n  method: put\n  operationId: ApplicationRegistry_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_ids.application_id}\n  method: get\n  operationId: ApplicationRegistry_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_ids.application_id}/api-keys\n  method: get\n  operationId: ApplicationAccess_ListAPIKeys\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_ids.application_id}/api-keys\n  method: post\n  operationId: ApplicationAccess_CreateAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_ids.application_id}/api-keys/{api_key.id}\n  method: put\n  operationId: ApplicationAccess_UpdateAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_ids.application_id}/api-keys/{key_id}\n\
  \  method: get\n  operationId: ApplicationAccess_GetAPIKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_ids.application_id}/api-keys/{key_id}\n  method: delete\n  operationId: ApplicationAccess_DeleteAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_ids.application_id}/collaborator/organization/{collaborator.organization_ids.organization_id}\n  method: get\n  operationId: ApplicationAccess_GetCollaborator2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_ids.application_id}/collaborator/organization/{collaborator_ids.organization_ids.organization_id}\n\
  \  method: delete\n  operationId: ApplicationAccess_DeleteCollaborator2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_ids.application_id}/collaborator/user/{collaborator.user_ids.user_id}\n  method: get\n  operationId: ApplicationAccess_GetCollaborator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_ids.application_id}/collaborator/user/{collaborator_ids.user_ids.user_id}\n  method: delete\n  operationId: ApplicationAccess_DeleteCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_ids.application_id}/collaborators\n  method: get\n  operationId: ApplicationAccess_ListCollaborators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_ids.application_id}/collaborators\n  method: put\n  operationId: ApplicationAccess_SetCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}\n  method: delete\n  operationId: ApplicationRegistry_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/dev-eui\n  method: post\n  operationId: ApplicationRegistry_IssueDevEUI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/purge\n  method: delete\n  operationId: ApplicationRegistry_Purge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/restore\n\
  \  method: post\n  operationId: ApplicationRegistry_Restore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/rights\n  method: get\n  operationId: ApplicationAccess_ListRights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{application_ids.application_id}/devices/batch\n  method: delete\n  operationId: AsEndDeviceBatchRegistry_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{application_ids.application_id}/devices/{device_id}\n  method: delete\n  operationId: AsEndDeviceRegistry_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{application_ids.application_id}/devices/{device_id}/down\n  method: get\n  operationId: AppAs_DownlinkQueueList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{application_ids.application_id}/devices/{device_id}/packages\n  method: get\n  operationId: ApplicationPackageRegistry_List\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{application_ids.application_id}/link\n  method: get\n  operationId: As_GetLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{application_ids.application_id}/link\n  method: put\n  operationId: As_SetLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{application_ids.application_id}/packages/associations/{f_port}\n  method: delete\n  operationId: ApplicationPackageRegistry_DeleteDefaultAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{application_ids.application_id}/packages/storage/{type}\n  method: get\n  operationId: ApplicationUpStorage_GetStoredApplicationUp2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{application_ids.application_id}/packages/storage/{type}/count\n  method: get\n  operationId: ApplicationUpStorage_GetStoredApplicationUpCount2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{application_id}/link\n  method: delete\n  operationId: As_DeleteLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{application_id}/link/stats\n  method: get\n  operationId: As_GetLinkStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{application_id}/mqtt-connection-info\n  method: get\n  operationId: AppAs_GetMQTTConnectionInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{association.ids.end_device_ids.application_ids.application_id}/devices/{association.ids.end_device_ids.device_id}/packages/associations/{association.ids.f_port}\n  method: put\n  operationId: ApplicationPackageRegistry_SetAssociation\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{default.ids.application_ids.application_id}/packages/associations/{default.ids.f_port}\n  method: put\n  operationId: ApplicationPackageRegistry_SetDefaultAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{end_device.ids.application_ids.application_id}/devices\n  method: post\n  operationId: AsEndDeviceRegistry_Set2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{end_device.ids.application_ids.application_id}/devices/{end_device.ids.device_id}\n  method: put\n  operationId: AsEndDeviceRegistry_Set\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}\n  method: get\n  operationId: AsEndDeviceRegistry_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}/down/decode\n\
  \  method: post\n  operationId: AppAs_DecodeDownlink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}/down/encode\n  method: post\n  operationId: AppAs_EncodeDownlink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}/down/push\n  method: post\n  operationId: AppAs_DownlinkQueuePush\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}/down/replace\n  method: post\n  operationId: AppAs_DownlinkQueueReplace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}/packages/associations/{f_port}\n  method: delete\n  operationId: ApplicationPackageRegistry_DeleteAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}/packages/storage/{type}\n  method: get\n  operationId: ApplicationUpStorage_GetStoredApplicationUp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}/packages/storage/{type}/count\n  method: get\n  operationId: ApplicationUpStorage_GetStoredApplicationUpCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}/up/decode\n\
  \  method: post\n  operationId: AppAs_DecodeUplink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}/up/simulate\n  method: post\n  operationId: AppAs_SimulateUplink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /as/applications/{ids.application_ids.application_id}/devices/{ids.device_id}/packages/associations\n  method: get\n  operationId: ApplicationPackageRegistry_ListAssociations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{ids.application_ids.application_id}/packages/associations/{ids.f_port}\n  method: get\n  operationId: ApplicationPackageRegistry_GetDefaultAssociation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{ids.application_id}/packages/associations\n  method: get\n  operationId: ApplicationPackageRegistry_ListDefaultAssociations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/applications/{ids.end_device_ids.application_ids.application_id}/devices/{ids.end_device_ids.device_id}/packages/associations/{ids.f_port}\n  method: get\n  operationId: ApplicationPackageRegistry_GetAssociation\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /as/configuration\n  method: get\n  operationId: As_GetConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /js/applications/{application_ids.application_id}/settings\n  method: get\n  operationId: ApplicationActivationSettingRegistry_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /js/applications/{application_ids.application_id}/settings\n  method: delete\n  operationId: ApplicationActivationSettingRegistry_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /js/applications/{application_ids.application_id}/settings\n  method: post\n  operationId: ApplicationActivationSettingRegistry_Set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{collaborator.organization_ids.organization_id}/applications\n  method: get\n  operationId: ApplicationRegistry_List3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{collaborator.organization_ids.organization_id}/applications\n  method: post\n  operationId: ApplicationRegistry_Create2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{collaborator.user_ids.user_id}/applications\n  method: get\n  operationId: ApplicationRegistry_List2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{collaborator.user_ids.user_id}/applications\n  method: post\n  operationId: ApplicationRegistry_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_ids.application_id}/devices\n  method: get\n  operationId: EndDeviceRegistry_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_ids.application_id}/devices/batch\n  method: get\n  operationId: EndDeviceBatchRegistry_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_ids.application_id}/devices/batch\n  method: delete\n  operationId: EndDeviceBatchRegistry_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_ids.application_id}/devices/count\n  method: get\n  operationId: EndDeviceRegistry_Count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /applications/{application_ids.application_id}/devices/filter\n  method: post\n  operationId: EndDeviceRegistry_List2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_ids.application_id}/devices/{device_id}\n  method: delete\n  operationId: EndDeviceRegistry_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{end_device.ids.application_ids.application_id}/devices\n  method: post\n  operationId: EndDeviceRegistry_Create\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{end_device.ids.application_ids.application_id}/devices/{end_device.ids.device_id}\n  method: put\n  operationId: EndDeviceRegistry_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{end_device_ids.application_ids.application_id}/devices/{end_device_ids.device_id}\n  method: get\n  operationId: EndDeviceRegistry_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /dr/applications/{application_ids.application_id}/brands\n  method: get\n  operationId: DeviceRepository_ListBrands2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/applications/{application_ids.application_id}/brands/{brand_id}\n  method: get\n  operationId: DeviceRepository_GetBrand2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/applications/{application_ids.application_id}/brands/{brand_id}/models\n  method: get\n  operationId: DeviceRepository_ListModels4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/applications/{application_ids.application_id}/brands/{brand_id}/models/{model_id}\n  method: get\n  operationId: DeviceRepository_GetModel2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/applications/{application_ids.application_id}/brands/{version_ids.brand_id}/models/{version_ids.model_id}/{version_ids.firmware_version}/{version_ids.band_id}/formatters/downlink/decoder\n  method: get\n  operationId: DeviceRepository_GetDownlinkDecoder2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/applications/{application_ids.application_id}/brands/{version_ids.brand_id}/models/{version_ids.model_id}/{version_ids.firmware_version}/{version_ids.band_id}/formatters/downlink/encoder\n  method: get\n  operationId: DeviceRepository_GetDownlinkEncoder2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/applications/{application_ids.application_id}/brands/{version_ids.brand_id}/models/{version_ids.model_id}/{version_ids.firmware_version}/{version_ids.band_id}/formatters/uplink/decoder\n\
  \  method: get\n  operationId: DeviceRepository_GetUplinkDecoder2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/applications/{application_ids.application_id}/brands/{version_ids.brand_id}/models/{version_ids.model_id}/{version_ids.firmware_version}/{version_ids.band_id}/template\n  method: get\n  operationId: DeviceRepository_GetTemplate3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/applications/{application_ids.application_id}/models\n  method: get\n  operationId: DeviceRepository_ListModels3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/applications/{application_ids.application_id}/vendors/{end_device_profile_ids.vendor_id}/profiles/{end_device_profile_ids.vendor_profile_id}/template\n\
  \  method: get\n  operationId: DeviceRepository_GetTemplate4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/brands\n  method: get\n  operationId: DeviceRepository_ListBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/brands/{brand_id}\n  method: get\n  operationId: DeviceRepository_GetBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/brands/{brand_id}/models\n  method: get\n  operationId: DeviceRepository_ListModels2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/brands/{brand_id}/models/{model_id}\n  method: get\n  operationId: DeviceRepository_GetModel\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/brands/{version_ids.brand_id}/models/{version_ids.model_id}/{version_ids.firmware_version}/{version_ids.band_id}/formatters/downlink/decoder\n  method: get\n  operationId: DeviceRepository_GetDownlinkDecoder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/brands/{version_ids.brand_id}/models/{version_ids.model_id}/{version_ids.firmware_version}/{version_ids.band_id}/formatters/downlink/encoder\n  method: get\n  operationId: DeviceRepository_GetDownlinkEncoder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/brands/{version_ids.brand_id}/models/{version_ids.model_id}/{version_ids.firmware_version}/{version_ids.band_id}/formatters/uplink/decoder\n\
  \  method: get\n  operationId: DeviceRepository_GetUplinkDecoder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/brands/{version_ids.brand_id}/models/{version_ids.model_id}/{version_ids.firmware_version}/{version_ids.band_id}/template\n  method: get\n  operationId: DeviceRepository_GetTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/models\n  method: get\n  operationId: DeviceRepository_ListModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dr/vendors/{end_device_profile_ids.vendor_id}/profiles/{end_device_profile_ids.vendor_profile_id}/template\n  method: get\n  operationId: DeviceRepository_GetTemplate2\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edcs/applications/{application_ids.application_id}/authorize\n  method: post\n  operationId: EndDeviceClaimingServer_AuthorizeApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edcs/applications/{application_id}/authorize\n  method: delete\n  operationId: EndDeviceClaimingServer_UnauthorizeApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /edcs/claim\n  method: post\n  operationId: EndDeviceClaimingServer_Claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edcs/claim/info\n  method: post\n  operationId: EndDeviceClaimingServer_GetInfoByJoinEUI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edcs/claim/info/batch\n  method: post\n  operationId: EndDeviceBatchClaimingServer_GetInfoByJoinEUIs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edcs/claim/{application_ids.application_id}/devices/batch\n  method: delete\n  operationId: EndDeviceBatchClaimingServer_Unclaim\n  x-agentic-access:\n    action-class: acting\n    cons\n\n# --- truncated at 32 KB (110 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/agentic-access/the-things-network-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-things-network/refs/heads/main/agentic-access/the-things-network-agentic-access.yml
summary_line: 329 operations · 174 acting · 3 human-in-the-loop
tags:
- LoRaWAN
- IoT
- Internet Of Things
- Open Source
- Network Server
- LPWAN
- Telemetry
- Sensors
- Gateways
- Connectivity
- Apache 2.0
---
