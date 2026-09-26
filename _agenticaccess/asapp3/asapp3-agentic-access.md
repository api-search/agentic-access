---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 30
api_specs:
- filename: asapp3-autocompose-api-openapi.yml
  format: yaml
  label: Asapp3 Auto Compose API
  slug: asapp3-autocompose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autocompose-api-openapi.yml
- filename: asapp3-autosummary-api-openapi.yml
  format: yaml
  label: Asapp3 Auto Summary API
  slug: asapp3-autosummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autosummary-api-openapi.yml
- filename: asapp3-autotranscribe-api-openapi.yml
  format: yaml
  label: Asapp3 Auto Transcribe API
  slug: asapp3-autotranscribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autotranscribe-api-openapi.yml
- filename: asapp3-autotranscribe-media-gateway-api-openapi.yml
  format: yaml
  label: Asapp3 AutoTranscribe Media Gateway API
  slug: asapp3-autotranscribe-media-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autotranscribe-media-gateway-api-openapi.yml
- filename: asapp3-conversations-api-openapi.yml
  format: yaml
  label: Asapp3 Conversations API
  slug: asapp3-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-conversations-api-openapi.yml
- filename: asapp3-file-exporter-api-openapi.yml
  format: yaml
  label: Asapp3 File Exporter API
  slug: asapp3-file-exporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-file-exporter-api-openapi.yml
- filename: asapp3-generativeagent-api-openapi.yml
  format: yaml
  label: Asapp3 Generative Agent API
  slug: asapp3-generativeagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-generativeagent-api-openapi.yml
- filename: asapp3-health-check-api-openapi.yml
  format: yaml
  label: Asapp3 Health Check API
  slug: asapp3-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-health-check-api-openapi.yml
- filename: asapp3-knowledge-base-api-openapi.yml
  format: yaml
  label: Asapp3 Knowledge Base API
  slug: asapp3-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-knowledge-base-api-openapi.yml
- filename: asapp3-metadata-api-openapi.yml
  format: yaml
  label: Asapp3 Metadata API
  slug: asapp3-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-metadata-api-openapi.yml
consequence_counts:
  read: 30
  safety-critical: 1
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Asapp3 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /mg-autotranscribe/v1/stop-streaming
operation_count: 56
overview: 'Asapp3 exposes 56 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 25 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Asapp3
provider_slug: asapp3
slug: asapp3-agentic-access
source_filename: asapp3-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: generated\nsource: openapi/asapp3-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    connected: 30\n    acting: 26\n  by_consequence:\n    read: 30\n    write: 25\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /autocompose/v1/conversations/{conversationId}/suggestions\n  method: post\n  operationId: getSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/profanity/evaluation\n  method: post\n  operationId: getEvaluation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/spellcheck/correction\n  method: post\n  operationId: getSpellingCorrection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/analytics/message-sent\n  method: post\n  operationId: createMessageSentEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/conversations/{conversationId}/message-analytic-events\n  method: post\n  operationId: createMessageAnalyticEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/responses/globals\n  method: get\n  operationId: getGlobalResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/responses/customs\n  method: get\n  operationId: getCustomResponseCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/responses/customs/folder\n  method: post\n  operationId: addCustomResponseFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/responses/customs/response\n  method: post\n  operationId: addCustomResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/responses/customs/response/{responseId}\n  method: put\n  operationId: updateCustomResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/responses/customs/response/{responseId}\n\
  \  method: delete\n  operationId: deleteCustomResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/responses/customs/folder/{folderId}\n  method: put\n  operationId: updateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/responses/customs/folder/{folderId}\n  method: delete\n  operationId: deleteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/autopilot/greetings\n  method: get\n  operationId: getAutopilotGreetings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/autopilot/greetings\n  method: put\n  operationId: updateAutopilotGreetings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/autopilot/greetings/status\n  method: get\n  operationId: getAutopilotGreetingsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/autopilot/greetings/status\n\
  \  method: put\n  operationId: updateAutopilotGreetingsStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autosummary/v1/intent/{conversationId}\n  method: get\n  operationId: getIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autosummary/v1/free-text-summaries/{conversationId}\n  method: get\n  operationId: getFreeTextSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autosummary/v1/feedback/free-text-summaries/{conversationId}\n  method: post\n  operationId: createFeedbackEvent\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autosummary/v1/free-text-summaries\n  method: post\n  operationId: retrieveFreeTextSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autosummary/v1/structured-data\n  method: post\n  operationId: retrieveStructuredData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autotranscribe/v1/streaming-url\n  method: post\n  operationId: getStreamingUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations\n  method:\
  \ post\n  operationId: createOrUpdateConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversation/v1/conversations\n  method: get\n  operationId: getConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}/messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversation/v1/conversations/{conversationId}/messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}/messages/{messageId}\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}/messages/batch\n  method: post\n  operationId: createBatchMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversation/v1/conversation/messages\n  method: get\n  operationId: getMessagesByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}/authenticate\n  method: post\n  operationId: postAuthenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fileexporter/v1/static/listfeeds\n  method: post\n  operationId: listFeeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeedversions\n\
  \  method: post\n  operationId: listFeedVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeedformats\n  method: post\n  operationId: listFeedFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeeddates\n  method: post\n  operationId: listFeedDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeedintervals\n  method: post\n  operationId: listFeedIntervals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeedfiles\n  method: post\n  operationId:\
  \ listFeedFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/getfeedfile\n  method: post\n  operationId: listFeedFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generativeagent/v1/analyze\n  method: post\n  operationId: postAnalyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generativeagent/v1/streams\n  method: post\n  operationId: postStreams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generativeagent/v1/state\n  method: get\n  operationId: getState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /knowledge-base/v1/submissions\n  method: post\n  operationId: createSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /knowledge-base/v1/submissions/{id}\n  method: get\n  operationId: getSubmission\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /knowledge-base/v1/articles/{id}\n  method: get\n  operationId: getArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata-ingestion/v1/single-agent-metadata\n  method: post\n  operationId: singleAgentMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata-ingestion/v1/many-agent-metadata\n  method: post\n  operationId: manyAgentMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata-ingestion/v1/single-convo-metadata\n  method: post\n  operationId: singleConvoMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata-ingestion/v1/many-convo-metadata\n  method: post\n  operationId: manyConversationMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata-ingestion/v1/single-customer-metadata\n  method: post\n  operationId: singleCustomerMetadata\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata-ingestion/v1/many-customer-metadata\n  method: post\n  operationId: manyCustomerMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mg-autotranscribe/v1/start-streaming\n  method: post\n  operationId: startStreaming\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /mg-autotranscribe/v1/stop-streaming\n  method: post\n  operationId: stopStreaming\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mg-autotranscribe/v1/twilio-media-stream-url\n  method: get\n  operationId: getTwilioMediaStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/agentic-access/asapp3-agentic-access.yml
summary_line: 56 operations · 26 acting · 1 human-in-the-loop
tags:
- AI
- CustomerExperience
- Enterprise
- ContactCenter
- Platform
- Company
---
