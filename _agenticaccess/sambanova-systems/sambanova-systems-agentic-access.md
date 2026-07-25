---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 3
api_specs:
- filename: sambanova-systems-audio-api-openapi.yml
  format: yaml
  label: SambaNova Systems Audio API
  slug: sambanova-systems-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-audio-api-openapi.yml
- filename: sambanova-systems-chat-completions-api-openapi.yml
  format: yaml
  label: SambaNova Systems Chat completions API
  slug: sambanova-systems-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-chat-completions-api-openapi.yml
- filename: sambanova-systems-completions-api-openapi.yml
  format: yaml
  label: SambaNova Systems Completions API
  slug: sambanova-systems-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-completions-api-openapi.yml
- filename: sambanova-systems-embeddings-api-openapi.yml
  format: yaml
  label: SambaNova Systems Embeddings API
  slug: sambanova-systems-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-embeddings-api-openapi.yml
- filename: sambanova-systems-file-management-api-openapi.yml
  format: yaml
  label: SambaNova Systems File Management API
  slug: sambanova-systems-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-file-management-api-openapi.yml
- filename: sambanova-systems-main-agent-api-openapi.yml
  format: yaml
  label: SambaNova Systems Main Agent API
  slug: sambanova-systems-main-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-main-agent-api-openapi.yml
- filename: sambanova-systems-main-agent-interactive-api-openapi.yml
  format: yaml
  label: SambaNova Systems Main Agent Interactive API
  slug: sambanova-systems-main-agent-interactive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-main-agent-interactive-api-openapi.yml
- filename: sambanova-systems-messages-api-openapi.yml
  format: yaml
  label: SambaNova Systems Messages API
  slug: sambanova-systems-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-messages-api-openapi.yml
- filename: sambanova-systems-models-api-openapi.yml
  format: yaml
  label: SambaNova Systems Models API
  slug: sambanova-systems-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-models-api-openapi.yml
- filename: sambanova-systems-responses-api-openapi.yml
  format: yaml
  label: SambaNova Systems Responses API
  slug: sambanova-systems-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-responses-api-openapi.yml
- filename: sambanova-systems-subagents-api-openapi.yml
  format: yaml
  label: SambaNova Systems Subagents API
  slug: sambanova-systems-subagents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-subagents-api-openapi.yml
- filename: sambanova-systems-subagents-interactive-api-openapi.yml
  format: yaml
  label: SambaNova Systems Subagents Interactive API
  slug: sambanova-systems-subagents-interactive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-subagents-interactive-api-openapi.yml
consequence_counts:
  read: 3
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sambanova Systems Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'SambaNova Systems exposes 21 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SambaNova Systems
provider_slug: sambanova-systems
slug: sambanova-systems-agentic-access
source_filename: sambanova-systems-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/sambanova-systems-agents-openapi-original.yml, openapi/sambanova-systems-cloud-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 18\n    connected: 3\n  by_consequence:\n    write: 18\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /agent/mainagent\n  method: post\n  operationId: main_agent_agent_mainagent_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/mainagent/interactive\n\
  \  method: post\n  operationId: main_agent_interactive_agent_mainagent_interactive_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/coding\n  method: post\n  operationId: coding_agent_agent_coding_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/coding/interactive\n  method: post\n  operationId: coding_agent_interactive_agent_coding_interactive_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/datascience\n  method: post\n  operationId: datascience_agent_and_report_agent_datascience_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/datascience/interactive\n  method: post\n  operationId: datascience_interactive_agent_datascience_interactive_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/deepresearch\n  method: post\n  operationId: deepresearch_agent_agent_deepresearch_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/deepresearch/interactive\n  method: post\n  operationId: deepresearch_interactive_agent_agent_deepresearch_interactive_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/financialanalysis\n  method: post\n  operationId: financial_analysis_agent_agent_financialanalysis_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/financialanalysis/interactive\n  method: post\n  operationId: financial_analysis_agent_interactive_agent_financialanalysis_interactive_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/files/{file_id}\n  method: get\n  operationId: download_agent_file_agent_files__file_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /responses\n  method: post\n  operationId: createResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/count_tokens\n  method: post\n  operationId: countMessageTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/translations\n  method: post\n  operationId: createTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: getModelList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model_id}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/agentic-access/sambanova-systems-agentic-access.yml
summary_line: 21 operations · 18 acting
tags:
- Company
- Ai
- Artificial Intelligence
- Machine Learning
- LLM
- Inference
- Generative AI
- API
- Agents
- Embeddings
---
