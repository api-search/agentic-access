---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 7
api_specs:
- filename: docsbot-ai-docsbot-chat-api-api-openapi.yml
  format: yaml
  label: docsbot-ai DocsBot Chat API
  slug: docsbot-ai-docsbot-chat-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsbot-ai/openapi/docsbot-ai-docsbot-chat-api-api-openapi.yml
- filename: docsbot-ai-libraries-api-openapi.yml
  format: yaml
  label: docsbot-ai Libraries API
  slug: docsbot-ai-libraries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsbot-ai/openapi/docsbot-ai-libraries-api-openapi.yml
- filename: docsbot-ai-teams-api-openapi.yml
  format: yaml
  label: docsbot-ai Teams API
  slug: docsbot-ai-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docsbot-ai/openapi/docsbot-ai-teams-api-openapi.yml
consequence_counts:
  read: 7
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Docsbot Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'docsbot-ai exposes 20 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: docsbot-ai
provider_slug: docsbot-ai
slug: docsbot-ai-agentic-access
source_filename: docsbot-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/docsbot-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 7\n    acting: 13\n  by_consequence:\n    read: 7\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: get__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{team_id}/bots/{bot_id}/voice\n  method: post\n  operationId: Create_Widget_Voice_WebRTC_Session_teams__team_id__bots__bot_id__voice_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/voice/{call_id}/tool-result\n  method: get\n  operationId: Get_Widget_Voice_Tool_Result_teams__team_id__bots__bot_id__voice__call_id__tool_result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{team_id}/bots/{bot_id}/ask\n  method: post\n  operationId: Question_and_Answer__legacy__teams__team_id__bots__bot_id__ask_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/chat\n  method: post\n  operationId: Chat_or_Question_and_Answer_teams__team_id__bots__bot_id__chat_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/rate/{answer_id}\n  method: put\n  operationId: Rate_an_answer_teams__team_id__bots__bot_id__rate__answer_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/support/{answer_id}\n  method: put\n  operationId: Log_a_support_request_teams__team_id__bots__bot_id__support__answer_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/search\n  method: post\n  operationId: Semantic_Search_teams__team_id__bots__bot_id__search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/fetch\n  method: post\n  operationId: Fetch_Document_teams__team_id__bots__bot_id__fetch_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /libraries\n  method: get\n  operationId: List_libraries_that_can_be_searched_libraries_get\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{team_id}/bots/{bot_id}/chat-agent\n  method: post\n  operationId: Chat_or_Question_and_Answer_Using_Retreival_Agent_teams__team_id__bots__bot_id__chat_agent_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/conversations/{conv_id}/escalate\n  method: put\n  operationId: Log_a_support_escalation_for_the_conversation_teams__team_id__bots__bot_id__conversations__conv_id__escalate_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/conversations/{conv_id}\n  method: put\n  operationId: Update_Metadata_of_conversation_teams__team_id__bots__bot_id__conversations__conv_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/conversations/{conv_id}/lead\n  method: post\n  operationId: Capture_lead_and_update_conversation_metadata_teams__team_id__bots__bot_id__conversations__conv_id__lead_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /teams/{team_id}/bots/{bot_id}/conversations/{conv_id}/summarize\n  method: get\n  operationId: Generate_conversation_summary_teams__team_id__bots__bot_id__conversations__conv_id__summarize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{team_id}/bots/{bot_id}/conversations/{conv_id}/ticket\n  method: get\n  operationId: Generate_support_ticket_from_conversation_teams__team_id__bots__bot_id__conversations__conv_id__ticket_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{team_id}/bots/{bot_id}/research\n  method: post\n  operationId: Start_Deep_Research_teams__team_id__bots__bot_id__research_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/research/{job_id}\n  method: post\n  operationId: Continue_Deep_Research_teams__team_id__bots__bot_id__research__job_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/{team_id}/bots/{bot_id}/research/{job_id}\n  method: get\n  operationId: Research_Job_Status_teams__team_id__bots__bot_id__research__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{team_id}/bots/{bot_id}/research/{job_id}\n  method: delete\n  operationId: Cancel_Deep_Research_teams__team_id__bots__bot_id__research__job_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/docsbot-ai/agentic-access/docsbot-ai-agentic-access.yml
summary_line: 20 operations · 13 acting
tags:
- Company
- Artificial Intelligence
- Chatbots
- Automation
- Customer Service
---
