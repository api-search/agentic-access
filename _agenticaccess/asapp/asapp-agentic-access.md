---
acting_count: 41
action_class_counts:
  acting: 41
  connected: 40
api_specs:
- filename: asapp-autocompose-api-openapi.yml
  format: yaml
  label: ASAPP AutoCompose API
  slug: asapp-autocompose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autocompose-api-openapi.yml
- filename: asapp-autosummary-api-openapi.yml
  format: yaml
  label: ASAPP AutoSummary API
  slug: asapp-autosummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autosummary-api-openapi.yml
- filename: asapp-autotranscribe-api-openapi.yml
  format: yaml
  label: ASAPP AutoTranscribe API
  slug: asapp-autotranscribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autotranscribe-api-openapi.yml
- filename: asapp-autotranscribe-media-gateway-api-openapi.yml
  format: yaml
  label: ASAPP AutoTranscribe Media Gateway API
  slug: asapp-autotranscribe-media-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autotranscribe-media-gateway-api-openapi.yml
- filename: asapp-configuration-api-openapi.yml
  format: yaml
  label: ASAPP Configuration API
  slug: asapp-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-configuration-api-openapi.yml
- filename: asapp-conversations-api-openapi.yml
  format: yaml
  label: ASAPP Conversations API
  slug: asapp-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-conversations-api-openapi.yml
- filename: asapp-disengage-api-openapi.yml
  format: yaml
  label: ASAPP Disengage API
  slug: asapp-disengage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-disengage-api-openapi.yml
- filename: asapp-engage-api-openapi.yml
  format: yaml
  label: ASAPP Engage API
  slug: asapp-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-engage-api-openapi.yml
- filename: asapp-file-exporter-api-openapi.yml
  format: yaml
  label: ASAPP File Exporter API
  slug: asapp-file-exporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-file-exporter-api-openapi.yml
- filename: asapp-generativeagent-api-openapi.yml
  format: yaml
  label: ASAPP GenerativeAgent API
  slug: asapp-generativeagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-generativeagent-api-openapi.yml
- filename: asapp-health-check-api-openapi.yml
  format: yaml
  label: ASAPP Health Check API
  slug: asapp-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-health-check-api-openapi.yml
- filename: asapp-knowledge-base-api-openapi.yml
  format: yaml
  label: ASAPP Knowledge Base API
  slug: asapp-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-knowledge-base-api-openapi.yml
- filename: asapp-metadata-api-openapi.yml
  format: yaml
  label: ASAPP Metadata API
  slug: asapp-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-metadata-api-openapi.yml
- filename: asapp-twilio-media-stream-api-openapi.yml
  format: yaml
  label: ASAPP Twilio Media Stream API
  slug: asapp-twilio-media-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-twilio-media-stream-api-openapi.yml
consequence_counts:
  physical: 3
  read: 40
  safety-critical: 1
  write: 37
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Asapp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /mg-autotranscribe/v1/stop-streaming
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /generativeagent/v1/call-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /generativeagent/v1/complete-transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /generativeagent/v1/lookup-transfer
operation_count: 81
overview: 'ASAPP exposes 81 API operations that an AI agent could call, of which 41 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read, 37 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ASAPP
provider_slug: asapp
slug: asapp-agentic-access
source_filename: asapp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/asapp-autocompose-api-openapi.yml, openapi/asapp-autosummary-api-openapi.yml,\n  openapi/asapp-autotranscribe-api-openapi.yml, openapi/asapp-autotranscribe-media-gateway-api-openapi.yml,\n  openapi/asapp-configuration-api-openapi.yml, openapi/asapp-conversations-api-openapi.yml,\n  openapi/asapp-disengage-api-openapi.yml, openapi/asapp-engage-api-openapi.yml, openapi/asapp-file-exporter-api-openapi.yml,\n  openapi/asapp-generativeagent-api-openapi.yml, openapi/asapp-health-check-api-openapi.yml,\n  openapi/asapp-knowledge-base-api-openapi.yml, openapi/asapp-metadata-api-openapi.yml, openapi/asapp-twilio-media-stream-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 81\n\
  \  by_action_class:\n    connected: 40\n    acting: 41\n  by_consequence:\n    read: 40\n    write: 37\n    safety-critical: 1\n    physical: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /autocompose/v1/conversations/{conversationId}/suggestions\n  method: post\n  operationId: getSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/profanity/evaluation\n  method: post\n  operationId: getEvaluation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/spellcheck/correction\n  method: post\n  operationId: getSpellingCorrection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/analytics/message-sent\n  method: post\n\
  \  operationId: createMessageSentEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/conversations/{conversationId}/message-analytic-events\n  method: post\n  operationId: createMessageAnalyticEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/responses/globals\n\
  \  method: get\n  operationId: getGlobalResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/responses/customs\n  method: get\n  operationId: getCustomResponseCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/responses/customs/folder\n  method: post\n  operationId: addCustomResponseFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/responses/customs/response\n  method: post\n  operationId: addCustomResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/responses/customs/response/{responseId}\n  method: put\n  operationId: updateCustomResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/responses/customs/response/{responseId}\n  method: delete\n  operationId: deleteCustomResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /autocompose/v1/responses/customs/folder/{folderId}\n  method: put\n  operationId: updateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/responses/customs/folder/{folderId}\n  method: delete\n  operationId: deleteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/autopilot/greetings\n  method: get\n  operationId: getAutopilotGreetings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /autocompose/v1/autopilot/greetings\n  method: put\n  operationId: updateAutopilotGreetings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompose/v1/autopilot/greetings/status\n  method: get\n  operationId: getAutopilotGreetingsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocompose/v1/autopilot/greetings/status\n  method: put\n  operationId: updateAutopilotGreetingsStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /autosummary/v1/intent/{conversationId}\n  method: get\n  operationId: getIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autosummary/v1/intent\n  method: post\n  operationId: createIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autosummary/v1/free-text-summaries/{conversationId}\n  method: get\n  operationId: getFreeTextSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autosummary/v1/feedback/free-text-summaries/{conversationId}\n  method: post\n  operationId: createFeedbackEvent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autosummary/v1/free-text-summaries\n  method: post\n  operationId: retrieveFreeTextSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autosummary/v1/structured-data\n  method: post\n  operationId: retrieveStructuredData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autotranscribe/v1/streaming-url\n  method: post\n  operationId: getStreamingUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /mg-autotranscribe/v1/start-streaming\n  method: post\n  operationId: startStreaming\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mg-autotranscribe/v1/stop-streaming\n  method: post\n  operationId: stopStreaming\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mg-autotranscribe/v1/twilio-media-stream-url\n  method: get\n  operationId: getTwilioMediaStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /configuration/v1/custom-vocabularies\n  method: get\n  operationId: getCustomVocabularyConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v1/custom-vocabularies\n  method: post\n  operationId: postCustomVocabularyConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/v1/custom-vocabularies/{customVocabularyId}\n  method: get\n  operationId: getCustomVocabularyConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v1/custom-vocabularies/{customVocabularyId}\n\
  \  method: delete\n  operationId: deleteCustomVocabularyConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/v1/redaction-entities\n  method: get\n  operationId: listRedactionEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v1/redaction-entities/{entityId}\n  method: get\n  operationId: getRedactionEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v1/redaction-entities/{entityId}\n  method: patch\n  operationId: updateRedactionEntity\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/v1/structured-data-fields\n  method: get\n  operationId: getStructuredDataFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v1/structured-data-fields\n  method: post\n  operationId: postStructuredDataField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/v1/structured-data-fields/{structuredDataFieldId}\n  method: get\n  operationId: getStructuredDataField\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v1/structured-data-fields/{structuredDataFieldId}\n  method: put\n  operationId: putStructuredDataField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/v1/structured-data-fields/{structuredDataFieldId}\n  method: delete\n  operationId: deleteStructuredDataField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/v1/segments\n  method: get\n  operationId:\
  \ getSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v1/segments\n  method: post\n  operationId: postSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/v1/segments/{segmentId}\n  method: get\n  operationId: getSegment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v1/segments/{segmentId}\n  method: patch\n  operationId: patchSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/v1/segments/{segmentId}\n  method: delete\n  operationId: deleteSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversation/v1/conversations\n  method: post\n  operationId: createOrUpdateConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversation/v1/conversations\n  method: get\n  operationId: getConversations\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}/messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversation/v1/conversations/{conversationId}/messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}/messages/{messageId}\n\
  \  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}/messages/batch\n  method: post\n  operationId: createBatchMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversation/v1/conversation/messages\n  method: get\n  operationId: getMessagesByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/v1/conversations/{conversationId}/authenticate\n  method: post\n  operationId: postAuthenticate\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mg-genagent/v1/disengage\n  method: post\n  operationId: disengage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mg-genagent/v1/engage\n  method: post\n  operationId: engage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fileexporter/v1/static/listfeeds\n  method: post\n  operationId:\
  \ listFeeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeedversions\n  method: post\n  operationId: listFeedVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeedformats\n  method: post\n  operationId: listFeedFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeeddates\n  method: post\n  operationId: listFeedDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeedintervals\n  method: post\n  operationId: listFeedIntervals\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/listfeedfiles\n  method: post\n  operationId: listFeedFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fileexporter/v1/static/getfeedfile\n  method: post\n  operationId: listFeedFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generativeagent/v1/analyze\n  method: post\n  operationId: postAnalyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generativeagent/v1/streams\n  method:\
  \ post\n  operationId: postStreams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generativeagent/v1/state\n  method: get\n  operationId: getState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generativeagent/v1/call-transfers\n  method: post\n  operationId: createCallTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generativeagent/v1/call-transfers/{callTransferId}\n\
  \  method: get\n  operationId: getCallTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generativeagent/v1/lookup-transfer\n  method: post\n  operationId: lookupCallTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generativeagent/v1/complete-transfer\n  method: post\n  operationId: completeCallTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: getV1Health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /knowledge-base/v1/submissions\n  method: post\n  operationId: createSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /knowledge-base/v1/submissions/{id}\n  method: get\n  operationId: getSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /knowledge-base/v1/articles/{id}\n  method: get\n  operationId: getArticle\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata-ingestion/v1/single-agent-metadata\n  method: post\n  operationId: singleAgentMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata-ingestion/v1/many-agent-metadata\n  method: post\n  operationId: manyAgentMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata-ingestion/v1/single-convo-metadata\n  method: post\n  operationId: singleConvoMetadata\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata-ingestion/v1/many-convo-metadata\n  method: post\n  operationId: manyConversationMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata-ingestion/v1/single-customer-metadata\n  method: post\n  operationId: singleCustomerMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /metadata-ingestion/v1/many-customer-metadata\n  method: post\n  operationId: manyCustomerMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mg-genagent/v1/twilio-media-stream-url\n  method: get\n  operationId: getTwilioMediaStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/agentic-access/asapp-agentic-access.yml
summary_line: 81 operations · 41 acting · 1 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Contact Center
- Customer Experience
- Customer Service
- Generative AI
- Agent Assist
- Speech Recognition
- Knowledge Base
---
