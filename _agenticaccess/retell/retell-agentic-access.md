---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 14
api_specs:
- filename: retell-openapi.yml
  format: yaml
  label: Agents
  slug: agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Retell LLM
  slug: retell-llm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Conversation Flow
  slug: conversation-flow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Phone Calls
  slug: phone-calls
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Web Calls
  slug: web-calls
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Phone Numbers
  slug: phone-numbers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Voices
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Knowledge Bases
  slug: knowledge-bases
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Batch Call
  slug: batch-call
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
- filename: retell-openapi.yml
  format: yaml
  label: Concurrency
  slug: concurrency
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-openapi.yml
consequence_counts:
  read: 14
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Retell Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 35
overview: 'Retell AI exposes 35 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Retell AI
provider_slug: retell
slug: retell-agentic-access
source_filename: retell-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/retell-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    acting: 21\n    connected: 14\n  by_consequence:\n    write: 21\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /create-agent\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-agent/{agent_id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list-agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update-agent/{agent_id}\n  method: patch\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-agent/{agent_id}\n  method: delete\n  operationId: deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /create-retell-llm\n  method: post\n  operationId: createRetellLLM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-retell-llm/{llm_id}\n  method: get\n  operationId: getRetellLLM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list-retell-llms\n  method: get\n  operationId: listRetellLLMs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update-retell-llm/{llm_id}\n  method: patch\n  operationId: updateRetellLLM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-retell-llm/{llm_id}\n  method: delete\n  operationId: deleteRetellLLM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create-conversation-flow\n  method: post\n  operationId: createConversationFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-conversation-flow/{conversation_flow_id}\n  method: get\n  operationId: getConversationFlow\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list-conversation-flows\n  method: get\n  operationId: listConversationFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update-conversation-flow/{conversation_flow_id}\n  method: patch\n  operationId: updateConversationFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-conversation-flow/{conversation_flow_id}\n  method: delete\n  operationId: deleteConversationFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/create-phone-call\n  method: post\n  operationId: createPhoneCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/create-web-call\n  method: post\n  operationId: createWebCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-call/{call_id}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list-calls\n  method: post\n  operationId: listCalls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create-batch-call\n  method: post\n  operationId: createBatchCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create-phone-number\n  method: post\n  operationId: createPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /import-phone-number\n  method: post\n  operationId: importPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-phone-number/{phone_number}\n  method: get\n  operationId: getPhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list-phone-numbers\n  method: get\n  operationId: listPhoneNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update-phone-number/{phone_number}\n  method:\
  \ patch\n  operationId: updatePhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-phone-number/{phone_number}\n  method: delete\n  operationId: deletePhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /list-voices\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-voice/{voice_id}\n  method: get\n  operationId: getVoice\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /create-knowledge-base\n  method: post\n  operationId: createKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-knowledge-base/{knowledge_base_id}\n  method: get\n  operationId: getKnowledgeBase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list-knowledge-bases\n  method: get\n  operationId: listKnowledgeBases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delete-knowledge-base/{knowledge_base_id}\n\
  \  method: delete\n  operationId: deleteKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /add-knowledge-base-sources/{knowledge_base_id}\n  method: post\n  operationId: addKnowledgeBaseSources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-knowledge-base-source/{knowledge_base_id}/source/{source_id}\n  method: delete\n  operationId: deleteKnowledgeBaseSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-concurrency\n  method: get\n  operationId: getConcurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/agentic-access/retell-agentic-access.yml
summary_line: 35 operations · 21 acting
tags:
- AI
- Voice
- Voice Agents
- Conversational AI
- Telephony
---
