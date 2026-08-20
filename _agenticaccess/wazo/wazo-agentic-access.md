---
acting_count: 540
action_class_counts:
  acting: 540
  connected: 392
api_specs:
- filename: wazo-auth-api-openapi.yml
  format: yaml
  label: Wazo Authentication API (wazo-auth)
  slug: wazo-authentication-api-wazo-auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-auth-api-openapi.yml
- filename: wazo-confd-api-openapi.yml
  format: yaml
  label: Wazo Configuration API (wazo-confd)
  slug: wazo-configuration-api-wazo-confd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-confd-api-openapi.yml
- filename: wazo-calld-api-openapi.yml
  format: yaml
  label: Wazo Call Control / Application API (wazo-calld)
  slug: wazo-call-control-application-api-wazo-calld
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-calld-api-openapi.yml
- filename: wazo-call-logd-api-openapi.yml
  format: yaml
  label: Wazo Call Detail Records API (wazo-call-logd)
  slug: wazo-call-detail-records-api-wazo-call-logd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-call-logd-api-openapi.yml
- filename: wazo-dird-api-openapi.yml
  format: yaml
  label: Wazo Directory & Contacts API (wazo-dird)
  slug: wazo-directory-contacts-api-wazo-dird
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-dird-api-openapi.yml
- filename: wazo-provd-api-openapi.yml
  format: yaml
  label: Wazo Phone Provisioning API (wazo-provd)
  slug: wazo-phone-provisioning-api-wazo-provd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-provd-api-openapi.yml
- filename: wazo-webhookd-api-openapi.yml
  format: yaml
  label: Wazo Webhooks API (wazo-webhookd)
  slug: wazo-webhooks-api-wazo-webhookd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-webhookd-api-openapi.yml
- filename: wazo-plugind-api-openapi.yml
  format: yaml
  label: Wazo Plugin Management API (wazo-plugind)
  slug: wazo-plugin-management-api-wazo-plugind
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-plugind-api-openapi.yml
- filename: wazo-agentd-api-openapi.yml
  format: yaml
  label: Wazo Call Centre Agent API (wazo-agentd)
  slug: wazo-call-centre-agent-api-wazo-agentd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-agentd-api-openapi.yml
- filename: wazo-chatd-api-openapi.yml
  format: yaml
  label: Wazo Presence & Chat API (wazo-chatd)
  slug: wazo-presence-chat-api-wazo-chatd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-chatd-api-openapi.yml
- filename: wazo-phoned-api-openapi.yml
  format: yaml
  label: Wazo Phone Directory & Service API (wazo-phoned)
  slug: wazo-phone-directory-service-api-wazo-phoned
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-phoned-api-openapi.yml
- filename: wazo-setupd-api-openapi.yml
  format: yaml
  label: Wazo Initial Setup API (wazo-setupd)
  slug: wazo-initial-setup-api-wazo-setupd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-setupd-api-openapi.yml
- filename: wazo-amid-api-openapi.yml
  format: yaml
  label: Wazo Asterisk Manager Interface API (wazo-amid)
  slug: wazo-asterisk-manager-interface-api-wazo-amid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-amid-api-openapi.yml
- filename: wazo-unattributed-asyncapi.yml
  format: yaml
  label: Wazo Websocket Event Stream (wazo-websocketd)
  slug: wazo-websocket-event-stream-wazo-websocketd
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/asyncapi/wazo-unattributed-asyncapi.yml
consequence_counts:
  physical: 11
  read: 392
  safety-critical: 26
  write: 503
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 26
kind: agentic-access
layout: agentic-access
method: generated
name: Wazo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agents/skills
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /agents/skills/{skill_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /agents/skills/{skill_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /agents/{agent_id}/skills/{skill_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /agents/{agent_id}/skills/{skill_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /applications/{application_uuid}/calls/{call_id}/hold/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /applications/{application_uuid}/calls/{call_id}/moh/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /applications/{application_uuid}/calls/{call_id}/mute/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /applications/{application_uuid}/calls/{call_id}/progress/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /applications/{application_uuid}/playbacks/{playback_uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /applications/{application_uuid}/snoops/{snoop_uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /calls/{call_id}/hold/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /calls/{call_id}/mute/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /calls/{call_id}/record/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /conferences/{conference_id}/record
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /endpoints/{endpoint_name}/hold/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /queues/skillrules
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /queues/skillrules/{skillrule_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /queues/skillrules/{skillrule_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /token/{token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users/import
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users/me/calls/{call_id}/hold/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users/me/calls/{call_id}/mute/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users/me/calls/{call_id}/record/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users/password/reset
operation_count: 932
overview: 'Wazo exposes 932 API operations that an AI agent could call, of which 540 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 392 read, 503 write, 11 physical, and 26 safety-critical.


  26 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wazo
provider_slug: wazo
slug: wazo-agentic-access
source_filename: wazo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: generated\nsource: openapi/wazo-agentd-api-openapi.yml, openapi/wazo-amid-api-openapi.yml, openapi/wazo-auth-api-openapi.yml,\n  openapi/wazo-call-logd-api-openapi.yml, openapi/wazo-calld-api-openapi.yml, openapi/wazo-chatd-api-openapi.yml,\n  openapi/wazo-confd-api-openapi.yml, openapi/wazo-dird-api-openapi.yml, openapi/wazo-phoned-api-openapi.yml,\n  openapi/wazo-plugind-api-openapi.yml, openapi/wazo-provd-api-openapi.yml, openapi/wazo-setupd-api-openapi.yml,\n  openapi/wazo-webhookd-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 932\n  by_action_class:\n    connected: 392\n    acting: 540\n  by_consequence:\n    read: 392\n    write: 503\n    safety-critical: 26\n    physical: 11\n  human_in_the_loop_required:\
  \ 26\noperations:\n- path: /agents/by-id/{agent_id}\n  method: get\n  operationId: get_agent_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/by-number/{agent_number}\n  method: get\n  operationId: get_agent_by_number\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/by-id/{agent_id}/login\n  method: post\n  operationId: login_agent_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/by-number/{agent_number}/login\n  method: post\n  operationId: login_agent_by_number\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/agents\n  method: get\n  operationId: get_user_agent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/agents/login\n  method: post\n  operationId: login_user_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/by-id/{agent_id}/logoff\n  method: post\n  operationId: logoff_agent_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/by-number/{agent_number}/logoff\n  method: post\n  operationId: logoff_agent_by_number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/agents/logoff\n  method: post\n  operationId: logoff_user_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/by-number/{agent_number}/pause\n  method: post\n  operationId: pause_agent_by_number\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/agents/pause\n  method: post\n  operationId: pause_user_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/by-number/{agent_number}/unpause\n  method: post\n  operationId: unpause_agent_by_number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /users/me/agents/unpause\n  method: post\n  operationId: unpause_user_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/by-id/{agent_id}/add\n  method: post\n  operationId: add_agent_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/by-id/{agent_id}/remove\n  method: post\n  operationId: remove_agent_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agent_id}/queues/{queue_id}/login\n  method: put\n  operationId: login_agent_to_queue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/agents/queues/{queue_id}/login\n  method: put\n  operationId: user_agent_login_to_queue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agent_id}/queues/{queue_id}/logoff\n  method: put\n  operationId: logoff_agent_from_queue\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/agents/queues/{queue_id}/logoff\n  method: put\n  operationId: user_agent_logoff_from_queue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents\n  method: get\n  operationId: get_agents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/logoff\n  method: post\n  operationId: logoff_agents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/relog\n  method: post\n  operationId: relog_agents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: get\n  operationId: get_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: patch\n  operationId: patchConfig\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /action/{action}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /action/Command\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: get\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid}/external/google\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid}/external/google\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/external/google\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/external/microsoft\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid}/external/microsoft\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/external/microsoft\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/external/mobile\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid}/external/mobile\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/external/mobile\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/external/mobile\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/external/mobile/sender_id\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /backends\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: patch\n  operationId: patchConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /emails/{email_uuid}/confirm\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/{email_uuid}/confirm\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/{auth_type}/config\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/{auth_type}/config\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /external/{auth_type}/config\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/{auth_type}/config\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/{auth_type}/users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid}/external\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_uuid}/policies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_uuid}/policies/{policy_uuid}\n  method: put\n  operationId: addGroupPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_uuid}/policies/{policy_uuid}\n  method: delete\n  operationId: removeGroupPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: post\n  operationId: createGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_uuid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_uuid}\n  method: delete\n  operationId: delete_group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_uuid}\n  method: put\n  operationId: editGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /idp\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /idp/{idp_type}/users\n  method: put\n  operationId: updateUsersIDP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /idp/{idp_type}/users/{user_uuid}\n  method: put\n  operationId: addUserIDP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /idp/{idp_type}/users/{user_uuid}\n  method: delete\n  operationId: removeIDPUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /backends/ldap\n  method: get\n  operationId: getLDAPBackendConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /backends/ldap\n \
  \ method: put\n  operationId: updateLDAPBackendConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /backends/ldap\n  method: delete\n  operationId: deleteLDAPBackendConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/password/reset\n  method: get\n  operationId: reset_password\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/password/reset\n  method: post\n  operationId: reset_password_change\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /policies\n  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies\n  method: post\n  operationId: createPolicies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policies/{policy_uuid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies/{policy_uuid}\n  method: delete\n  operationId: delete_policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policies/{policy_uuid}\n  method: put\n  operationId: editPolicies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policies/{policy_uuid}/acl/{access}\n  method: delete\n  operationId: deletePolicyAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policies/{policy_uuid}/acl/{access}\n  method: put\n  operationId: addPolicyAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saml/sso\n  method: post\n  operationId: samlSSO\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saml/acs\n  method: post\n  operationId: processACS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saml/logout\n  method: get\n  operationId: samlLogout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saml/sls\n  method: get\n  operationId: samlLogoutResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /backends/saml\n  method: delete\n  operationId: deleteSAMLBackendConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /backends/saml\n\
  \  method: get\n  operationId: getSAMLBackendConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /backends/saml\n  method: post\n  operationId: createSAMLBackendConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /backends/saml\n  method: put\n  operationId: updateSAMLBackendConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /backends/saml/metadata\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /backends/saml/acs_url_template\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_uuid}\n  method: delete\n  operationId: delete_session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants\n  method: post\n  operationId: createTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_uuid}\n  method: delete\n  operationId: delete_tenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_uuid}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_uuid}\n  method: put\n  operationId: updateTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_uuid}/domains\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_uuid}/parent/{parent_tenant_uuid}\n  method: put\n  operationId: updateTenantParent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token/{token}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/{token}\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/{token}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /token/{token}/scopes/check\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens\n  method: get\n  operationId: listRefreshTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid_or_me}/tokens\n  method: get\n  operationId: listUserRefreshTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid_or_me}/tokens/{client_id}\n  method: delete\n  operationId: deleteRefreshTokens\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{user_uuid}/emails\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/emails\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/emails/{email_uuid}/confirm\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_uuid}/users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_uuid}/users/{user_uuid}\n  method: put\n  operationId: addUserGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_uuid}/users/{user_uuid}\n  method: delete\n  operationId: removeUserGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/groups\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid}/policies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_uuid}/policies/{policy_uuid}\n  method: put\n  operationId: addUserPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_uuid}/policies/{policy_uuid}\n  method: delete\n  operationId: removeUserPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      trig\n\n# --- truncated at 32 KB (264 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/agentic-access/wazo-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/agentic-access/wazo-agentic-access.yml
summary_line: 932 operations · 540 acting · 26 human-in-the-loop
tags:
- Telephony
- VoIP
- Unified Communications
- UCaaS
- Contact Center
- SIP
- asterisk
- WebRTC
- Open-Source
- Self-Hosted
- White Label
- PBX
- MSP
- Call Center
- Provisioning
- Webhook
- Event-Driven
- Chat
- Presence
- CDR
---
