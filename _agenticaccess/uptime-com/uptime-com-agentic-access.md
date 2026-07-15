---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 17
api_specs:
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Checks & Monitors API
  slug: checks-monitors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Outages API
  slug: outages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com SLA Reports API
  slug: sla-reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Status Pages API
  slug: status-pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Contacts & Integrations API
  slug: contacts-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Tags API
  slug: tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
consequence_counts:
  read: 17
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uptime Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 39
overview: 'Uptime.com exposes 39 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 22 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Uptime.com
provider_slug: uptime-com
slug: uptime-com-agentic-access
source_filename: uptime-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/uptime-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 17\n    acting: 22\n  by_consequence:\n    read: 17\n    write: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /checks/\n  method: get\n  operationId: listChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checks/add-http/\n  method: post\n  operationId: createHttpCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checks/add-api/\n  method: post\n  operationId: createApiCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checks/{pk}/\n  method: get\n  operationId: getCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checks/{pk}/\n  method: patch\n  operationId: updateCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /checks/{pk}/\n  method: delete\n  operationId: deleteCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checks/{pk}/pause/\n  method: post\n  operationId: pauseCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checks/{pk}/resume/\n  method: post\n  operationId: resumeCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /checks/{pk}/stats/\n  method: get\n  operationId: getCheckStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outages/\n  method: get\n  operationId: listOutages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outages/{pk}/\n  method: get\n  operationId: getOutage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sla/report/\n  method: get\n  operationId: listSlaReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sla/report/\n  method: post\n  operationId: createSlaReport\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sla/report/{pk}/\n  method: get\n  operationId: getSlaReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sla/report/{pk}/\n  method: patch\n  operationId: updateSlaReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sla/report/{pk}/\n  method: delete\n  operationId: deleteSlaReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statuspages/\n  method: get\n  operationId: listStatusPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statuspages/\n  method: post\n  operationId: createStatusPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statuspages/{pk}/\n  method: get\n  operationId: getStatusPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statuspages/{pk}/\n  method: patch\n  operationId:\
  \ updateStatusPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statuspages/{pk}/\n  method: delete\n  operationId: deleteStatusPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statuspages/{statuspage_pk}/incidents/\n  method: get\n  operationId: listStatusPageIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statuspages/{statuspage_pk}/incidents/\n  method: post\n  operationId: createStatusPageIncident\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statuspages/{statuspage_pk}/components/\n  method: get\n  operationId: listStatusPageComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statuspages/{statuspage_pk}/components/\n  method: post\n  operationId: createStatusPageComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact-groups/\n  method: get\n  operationId: listContactGroups\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact-groups/\n  method: post\n  operationId: createContactGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact-groups/{pk}/\n  method: get\n  operationId: getContactGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact-groups/{pk}/\n  method: patch\n  operationId: updateContactGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /contact-groups/{pk}/\n  method: delete\n  operationId: deleteContactGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/\n  method: post\n  operationId: createIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/{pk}/\n\
  \  method: get\n  operationId: getIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/{pk}/\n  method: delete\n  operationId: deleteIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-tags/\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-tags/\n  method: post\n  operationId: createTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-tags/{pk}/\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-tags/{pk}/\n  method: patch\n  operationId: updateTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check-tags/{pk}/\n  method: delete\n  operationId: deleteTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/agentic-access/uptime-com-agentic-access.yml
summary_line: 39 operations · 22 acting
tags:
- Monitoring
- Uptime
- Website Monitoring
- Status Pages
- SLA
---
