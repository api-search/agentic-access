---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 25
api_specs:
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Account API
  slug: dotloop-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Profiles API
  slug: dotloop-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loops API
  slug: dotloop-loops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loop Details API
  slug: dotloop-loop-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loop-It API
  slug: dotloop-loop-it-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Folders API
  slug: dotloop-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Documents API
  slug: dotloop-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Participants API
  slug: dotloop-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Tasks API
  slug: dotloop-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Activities API
  slug: dotloop-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Contacts API
  slug: dotloop-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loop Templates API
  slug: dotloop-loop-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Webhooks API
  slug: dotloop-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
consequence_counts:
  read: 25
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dotloop Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 43
overview: 'dotloop exposes 43 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: dotloop
provider_slug: dotloop
slug: dotloop-agentic-access
source_filename: dotloop-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dotloop-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 25\n    acting: 18\n  by_consequence:\n    read: 25\n    write: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: listProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: post\n  operationId: createProfile\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}\n  method: patch\n  operationId: updateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop\n  method: get\n  operationId: listLoops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop\n  method: post\n  operationId: createLoop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop/{loop_id}\n  method: get\n  operationId: getLoop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}\n  method: patch\n  operationId: updateLoop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /profile/{profile_id}/loop/{loop_id}/detail\n  method: get\n  operationId: getLoopDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/detail\n  method: patch\n  operationId: updateLoopDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loop-it\n  method: post\n  operationId: loopIt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop/{loop_id}/folder\n\
  \  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/folder\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop/{loop_id}/folder/{folder_id}\n  method: get\n  operationId: getFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/folder/{folder_id}\n  method: patch\n  operationId: updateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop/{loop_id}/folder/{folder_id}/document\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/folder/{folder_id}/document\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop/{loop_id}/folder/{folder_id}/document/{document_id}\n  method: get\n  operationId: getDocument\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/participant\n  method: get\n  operationId: listParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/participant\n  method: post\n  operationId: addParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop/{loop_id}/participant/{participant_id}\n  method: get\n  operationId: getParticipant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/participant/{participant_id}\n  method: patch\n  operationId: updateParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop/{loop_id}/participant/{participant_id}\n  method: delete\n  operationId: removeParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop/{loop_id}/tasklist\n  method: get\n  operationId: listTaskLists\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/tasklist/{task_list_id}\n  method: get\n  operationId: getTaskList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/tasklist/{task_list_id}/task\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/tasklist/{task_list_id}/task/{task_list_item_id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop/{loop_id}/activity\n  method: get\n  operationId: listActivities\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/{contact_id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact/{contact_id}\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/{contact_id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{profile_id}/loop-template\n  method: get\n  operationId: listLoopTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/{profile_id}/loop-template/{loop_template_id}\n  method: get\n  operationId: getLoopTemplate\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription/{subscription_id}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription/{subscription_id}\n  method: patch\n  operationId: updateSubscription\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription/{subscription_id}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription/{subscription_id}/event\n  method: get\n  operationId: listSubscriptionEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription/{subscription_id}/event/{event_id}\n  method: get\n  operationId: getSubscriptionEvent\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/agentic-access/dotloop-agentic-access.yml
summary_line: 43 operations · 18 acting
tags:
- Real Estate
- Transaction Management
- Loops
- Documents
- E-Signature
- Zillow Group
---
