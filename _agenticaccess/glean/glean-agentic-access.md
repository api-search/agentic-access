---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 26
api_specs:
- filename: glean-activity-api-openapi.yml
  format: yaml
  label: Glean Activity API
  slug: glean-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-activity-api-openapi.yml
- filename: glean-agents-api-openapi.yml
  format: yaml
  label: Glean Agents API
  slug: glean-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-agents-api-openapi.yml
- filename: glean-announcements-api-openapi.yml
  format: yaml
  label: Glean Announcements API
  slug: glean-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-announcements-api-openapi.yml
- filename: glean-answers-api-openapi.yml
  format: yaml
  label: Glean Answers API
  slug: glean-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-answers-api-openapi.yml
- filename: glean-chat-api-openapi.yml
  format: yaml
  label: Glean Chat API
  slug: glean-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-chat-api-openapi.yml
- filename: glean-collections-api-openapi.yml
  format: yaml
  label: Glean Collections API
  slug: glean-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-collections-api-openapi.yml
- filename: glean-documents-api-openapi.yml
  format: yaml
  label: Glean Documents API
  slug: glean-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-documents-api-openapi.yml
- filename: glean-governance-api-openapi.yml
  format: yaml
  label: Glean Governance API
  slug: glean-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-governance-api-openapi.yml
- filename: glean-insights-api-openapi.yml
  format: yaml
  label: Glean Insights API
  slug: glean-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-insights-api-openapi.yml
- filename: glean-people-api-openapi.yml
  format: yaml
  label: Glean People API
  slug: glean-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-people-api-openapi.yml
- filename: glean-pins-api-openapi.yml
  format: yaml
  label: Glean Pins API
  slug: glean-pins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-pins-api-openapi.yml
- filename: glean-search-api-openapi.yml
  format: yaml
  label: Glean Search API
  slug: glean-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-search-api-openapi.yml
- filename: glean-shortcuts-api-openapi.yml
  format: yaml
  label: Glean Shortcuts API
  slug: glean-shortcuts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-shortcuts-api-openapi.yml
- filename: glean-summarize-api-openapi.yml
  format: yaml
  label: Glean Summarize API
  slug: glean-summarize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-summarize-api-openapi.yml
- filename: glean-tools-api-openapi.yml
  format: yaml
  label: Glean Tools API
  slug: glean-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-tools-api-openapi.yml
- filename: glean-verification-api-openapi.yml
  format: yaml
  label: Glean Verification API
  slug: glean-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/openapi/glean-verification-api-openapi.yml
consequence_counts:
  physical: 1
  read: 26
  write: 34
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Glean Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chat
operation_count: 61
overview: 'Glean exposes 61 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 34 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Glean
provider_slug: glean
slug: glean-agentic-access
source_filename: glean-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/glean-activity-api-openapi.yml, openapi/glean-agents-api-openapi.yml, openapi/glean-announcements-api-openapi.yml,\n  openapi/glean-answers-api-openapi.yml, openapi/glean-chat-api-openapi.yml, openapi/glean-collections-api-openapi.yml,\n  openapi/glean-documents-api-openapi.yml, openapi/glean-governance-api-openapi.yml, openapi/glean-insights-api-openapi.yml,\n  openapi/glean-people-api-openapi.yml, openapi/glean-pins-api-openapi.yml, openapi/glean-search-api-openapi.yml,\n  openapi/glean-shortcuts-api-openapi.yml, openapi/glean-summarize-api-openapi.yml, openapi/glean-tools-api-openapi.yml,\n  openapi/glean-verification-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations:\
  \ 61\n  by_action_class:\n    acting: 35\n    connected: 26\n  by_consequence:\n    write: 34\n    read: 26\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /activity\n  method: post\n  operationId: activity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feedback\n  method: post\n  operationId: feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agent_id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}/schemas\n  method: get\n  operationId: getAgentSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/search\n  method: post\n  operationId: searchAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/runs/wait\n  method: post\n  operationId: runAgentWait\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/runs/stream\n  method: post\n  operationId: runAgentStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /createannouncement\n  method: post\n  operationId: createAnnouncement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /updateannouncement\n  method: post\n  operationId: updateAnnouncement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteannouncement\n  method: post\n  operationId: deleteAnnouncement\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /createanswer\n  method: post\n  operationId: createAnswer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /editanswer\n  method: post\n  operationId: editAnswer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteanswer\n  method: post\n\
  \  operationId: deleteAnswer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getanswer\n  method: post\n  operationId: getAnswer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listanswers\n  method: post\n  operationId: listAnswers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat\n  method: post\n  operationId: chat\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getchat\n  method: post\n  operationId: getChat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listchats\n  method: post\n  operationId: listChats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deletechats\n  method: post\n  operationId: deleteChats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteallchats\n  method: post\n  operationId: deleteAllChats\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploadchatfiles\n  method: post\n  operationId: uploadChatFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getchatfiles\n  method: post\n  operationId: getChatFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deletechatfiles\n  method: post\n  operationId: deleteChatFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /createcollection\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /editcollection\n  method: post\n  operationId: editCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deletecollection\n  method: post\n  operationId: deleteCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getcollection\n  method: post\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listcollections\n  method: post\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addcollectionitems\n  method: post\n  operationId: addCollectionItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /editcollectionitem\n\
  \  method: post\n  operationId: editCollectionItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deletecollectionitem\n  method: post\n  operationId: deleteCollectionItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getdocuments\n  method: post\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getdocumentsbyfacets\n  method: post\n  operationId: getDocumentsByFacets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getdocpermissions\n  method: post\n  operationId: getDocPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /governance/data/policies\n  method: post\n  operationId: createGovernancePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /governance/data/policies/{id}\n  method: get\n  operationId: getGovernancePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /governance/data/reports\n  method: post\n\
  \  operationId: createGovernanceReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights\n  method: post\n  operationId: insights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people\n  method: post\n  operationId: people\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{person_id}/photo\n\
  \  method: get\n  operationId: getPersonPhoto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pin\n  method: post\n  operationId: pin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unpin\n  method: post\n  operationId: unpin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getpin\n  method: post\n  operationId: getPin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /editpin\n  method: post\n  operationId: editPin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listpins\n  method: post\n  operationId: listPins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adminsearch\n  method: post\n  operationId: adminSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /autocomplete\n  method: post\n  operationId: autocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recommendations\n  method: post\n  operationId: recommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed\n  method: post\n  operationId: feed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /createshortcut\n  method: post\n  operationId: createShortcut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /updateshortcut\n\
  \  method: post\n  operationId: updateShortcut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteshortcut\n  method: post\n  operationId: deleteShortcut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getshortcut\n  method: post\n  operationId: getShortcut\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listshortcuts\n  method: post\n  operationId: listShortcuts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summarize\n  method: post\n  operationId: summarize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/list\n  method: post\n  operationId: listTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/call\n  method: post\n  operationId: callTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify\n\
  \  method: post\n  operationId: verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listverifications\n  method: post\n  operationId: listVerifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addverificationreminder\n  method: post\n  operationId: addVerificationReminder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/agentic-access/glean-agentic-access.yml
summary_line: 61 operations · 35 acting
tags:
- Agents
- Artificial Intelligence
- Answers
- Chat
- Connectors
- Enterprise Search
- Generative AI
- Indexing
- Knowledge
- RAG
- Search
- Work Assistant
---
