---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 17
api_specs:
- filename: mention-accounts-api-openapi.yml
  format: yaml
  label: Mention Accounts API
  slug: mention-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-accounts-api-openapi.yml
- filename: mention-alerts-api-openapi.yml
  format: yaml
  label: Mention Alerts API
  slug: mention-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-alerts-api-openapi.yml
- filename: mention-authors-api-openapi.yml
  format: yaml
  label: Mention Authors API
  slug: mention-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-authors-api-openapi.yml
- filename: mention-mentions-api-openapi.yml
  format: yaml
  label: Mention Mentions API
  slug: mention-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-mentions-api-openapi.yml
- filename: mention-shares-api-openapi.yml
  format: yaml
  label: Mention Shares API
  slug: mention-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-shares-api-openapi.yml
- filename: mention-stats-api-openapi.yml
  format: yaml
  label: Mention Stats API
  slug: mention-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-stats-api-openapi.yml
- filename: mention-tags-api-openapi.yml
  format: yaml
  label: Mention Tags API
  slug: mention-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-tags-api-openapi.yml
- filename: mention-tasks-api-openapi.yml
  format: yaml
  label: Mention Tasks API
  slug: mention-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-tasks-api-openapi.yml
- filename: mention-app-api-openapi.yml
  format: yaml
  label: Mention App API
  slug: mention-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/openapi/mention-app-api-openapi.yml
consequence_counts:
  read: 17
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mention Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'Mention exposes 36 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mention
provider_slug: mention
slug: mention-agentic-access
source_filename: mention-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/mention-accounts-api-openapi.yml, openapi/mention-alerts-api-openapi.yml, openapi/mention-app-api-openapi.yml,\n  openapi/mention-authors-api-openapi.yml, openapi/mention-mentions-api-openapi.yml, openapi/mention-shares-api-openapi.yml,\n  openapi/mention-stats-api-openapi.yml, openapi/mention-tags-api-openapi.yml, openapi/mention-tasks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 19\n    connected: 17\n  by_consequence:\n    write: 19\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}\n\
  \  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts\n  method: get\n  operationId: listAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts\n  method: post\n  operationId: createAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}\n  method: get\n  operationId: getAlert\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}\n  method: put\n  operationId: updateAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/pause\n  method: post\n  operationId: pauseAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/unpause\n  method: post\n  operationId: unpauseAlert\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/preferences\n  method: get\n  operationId: getAlertPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/preferences\n  method: put\n  operationId: updateAlertPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/data\n  method: get\n  operationId: getAppData\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/authors\n  method: get\n  operationId: listAuthors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/mentions\n  method: get\n  operationId: listMentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/mentions/{mention_id}\n  method: get\n  operationId: getMention\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/mentions/{mention_id}\n  method: put\n  operationId: curateMention\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/mentions/{mention_id}/children\n  method: get\n  operationId: getMentionChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/mentions/markallread\n  method: post\n  operationId: markAllMentionsRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/mentions\n  method: get\n  operationId:\
  \ streamMentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/shares\n  method: get\n  operationId: listAlertShares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/shares\n  method: post\n  operationId: createAlertShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/shares/{share_id}\n  method: get\n  operationId: getShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/shares/{share_id}\n  method: put\n  operationId: updateShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/shares/{share_id}\n  method: delete\n  operationId: deleteShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/tags\n  method: get\n  operationId: listAlertTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/tags\n  method: post\n  operationId: createAlertTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/tags/{tag_id}\n  method: put\n  operationId: renameTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/tags/{tag_id}\n  method: delete\n  operationId: deleteTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/tasks\n  method: get\n  operationId: listAlertTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/mentions/{mention_id}/tasks\n  method: post\n  operationId: createMentionTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/mentions/{mention_id}/tasks/{task_id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/alerts/{alert_id}/mentions/{mention_id}/tasks/{task_id}\n  method: put\n  operationId: updateTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/alerts/{alert_id}/mentions/{mention_id}/tasks/{task_id}\n  method: delete\n  operationId: deleteTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mention/refs/heads/main/agentic-access/mention-agentic-access.yml
summary_line: 36 operations · 19 acting
tags:
- Alerts
- Brand Monitoring
- Media Monitoring
- Social Listening
- Social Media
- Sentiment Analysis
- Reputation Management
- Influencer Marketing
- Competitive Intelligence
- Streaming
- Marketing
---
