---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 22
api_specs:
- filename: venice-ai-api-keys-api-openapi.yml
  format: yaml
  label: Venice.ai API Keys API
  slug: venice-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-api-keys-api-openapi.yml
- filename: venice-ai-audio-api-openapi.yml
  format: yaml
  label: Venice.ai Audio API
  slug: venice-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-audio-api-openapi.yml
- filename: venice-ai-augment-api-openapi.yml
  format: yaml
  label: Venice.ai Augment API
  slug: venice-ai-augment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-augment-api-openapi.yml
- filename: venice-ai-billing-api-openapi.yml
  format: yaml
  label: Venice.ai Billing API
  slug: venice-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-billing-api-openapi.yml
- filename: venice-ai-characters-api-openapi.yml
  format: yaml
  label: Venice.ai Characters API
  slug: venice-ai-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-characters-api-openapi.yml
- filename: venice-ai-crypto-rpc-api-openapi.yml
  format: yaml
  label: Venice.ai Crypto RPC API
  slug: venice-ai-crypto-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-crypto-rpc-api-openapi.yml
- filename: venice-ai-decisions-api-openapi.yml
  format: yaml
  label: Venice.ai Decisions API
  slug: venice-ai-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-decisions-api-openapi.yml
- filename: venice-ai-embeddings-api-openapi.yml
  format: yaml
  label: Venice.ai Embeddings API
  slug: venice-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-embeddings-api-openapi.yml
- filename: venice-ai-image-api-openapi.yml
  format: yaml
  label: Venice.ai Image API
  slug: venice-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-image-api-openapi.yml
- filename: venice-ai-models-api-openapi.yml
  format: yaml
  label: Venice.ai Models API
  slug: venice-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-models-api-openapi.yml
- filename: venice-ai-preview-api-openapi.yml
  format: yaml
  label: Venice.ai Preview API
  slug: venice-ai-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-preview-api-openapi.yml
- filename: venice-ai-responses-api-openapi.yml
  format: yaml
  label: Venice.ai Responses API
  slug: venice-ai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-responses-api-openapi.yml
- filename: venice-ai-speech-api-openapi.yml
  format: yaml
  label: Venice.ai Speech API
  slug: venice-ai-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-speech-api-openapi.yml
- filename: venice-ai-transcriptions-api-openapi.yml
  format: yaml
  label: Venice.ai Transcriptions API
  slug: venice-ai-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-transcriptions-api-openapi.yml
- filename: venice-ai-video-api-openapi.yml
  format: yaml
  label: Venice.ai Video API
  slug: venice-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-video-api-openapi.yml
- filename: venice-ai-voices-api-openapi.yml
  format: yaml
  label: Venice.ai Voices API
  slug: venice-ai-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-voices-api-openapi.yml
- filename: venice-ai-x402-api-openapi.yml
  format: yaml
  label: Venice.ai X402 API
  slug: venice-ai-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-x402-api-openapi.yml
- filename: venice-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Venice.ai Chat Completions API
  slug: venice-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-chat-completions-api-openapi.yml
consequence_counts:
  read: 22
  write: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Venice Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 55
overview: 'Venice.ai exposes 55 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 33 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Venice.ai
provider_slug: venice-ai
slug: venice-ai-agentic-access
source_filename: venice-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/venice-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    acting: 33\n    connected: 22\n  by_consequence:\n    write: 33\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /responses\n  method: post\n  operationId: createResponse\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image/generate\n  method: post\n  operationId: generateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generations\n  method: post\n  operationId: simpleGenerateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image/styles\n  method: get\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /image/upscale\n  method: post\n  operationId: upscaleImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image/edit\n  method: post\n  operationId: editImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image/multi-edit\n  method: post\n  operationId: multiEditImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image/background-remove\n  method: post\n  operationId: backgroundRemoveImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/traits\n  method: get\n  operationId: listModelTraits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/compatibility_mapping\n  method: get\n\
  \  operationId: listModelCompatibilityMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys\n  method: get\n  operationId: getApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys\n  method: patch\n  operationId: updateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys/{id}\n  method: get\n  operationId: getApiKeyById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys/rate_limits\n  method: get\n  operationId: getApiKeyRateLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys/rate_limits/log\n  method: get\n  operationId: getApiKeyRateLimitLogs\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys/generate_web3_key\n  method: get\n  operationId: getApiKeyGenerateWeb3Key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys/generate_web3_key\n  method: post\n  operationId: postApiKeyGenerateWeb3Key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /characters\n  method: get\n  operationId: listCharacters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /characters/{slug}\n  method: get\n  operationId: getCharacterBySlug\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /characters/{slug}/reviews\n  method: get\n  operationId: getCharacterReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decisions\n  method: post\n  operationId: createDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /systemone\n  method: post\n  operationId: createDecisionSystemOne\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/speech\n  method: post\n  operationId: createSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/voices\n  method: post\n  operationId: createClonedVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/complete\n  method: post\n  operationId: completeVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/queue\n  method: post\n  operationId: queueVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/quote\n  method: post\n  operationId: quoteVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/retrieve\n  method: post\n  operationId: retrieveVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/transcriptions\n  method: post\n  operationId: createVideoTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /augment/text-parser\n  method: post\n  operationId: createTextParser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/complete\n  method: post\n  operationId: completeAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/queue\n  method: post\n  operationId: queueAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/quote\n  method: post\n  operationId: quoteAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/retrieve\n  method: post\n  operationId: retrieveAudio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audio/voice-changer/queue\n  method: post\n  operationId: queueVoiceChanger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /audio/voice-changer/quote\n  method: post\n  operationId: quoteVoiceChanger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/voice-changer/retrieve\n  method: post\n  operationId: retrieveVoiceChanger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audio/voice-changer/complete\n  method: post\n  operationId: completeVoiceChanger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /billing/balance\n  method: get\n  operationId: getBillingBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage\n  method: get\n  operationId: getBillingUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage-analytics\n  method: get\n  operationId: getBillingUsageAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage-history\n  method: get\n  operationId: getBillingUsageHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crypto/rpc/networks\n  method: get\n  operationId: listCryptoRpcNetworks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crypto/rpc/{network}\n  method: post\n  operationId: cryptoRpcProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/balance/{walletAddress}\n  method: get\n  operationId: getX402Balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/top-up\n  method: post\n  operationId: topUpX402Balance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/transactions/{walletAddress}\n  method: get\n  operationId: getX402Transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /augment/scrape\n  method: post\n  operationId: webScrape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /augment/search\n  method: post\n  operationId: webSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/agentic-access/venice-ai-agentic-access.yml
summary_line: 55 operations · 33 acting
tags:
- Company
- Artificial Intelligence
- LLM
- Image Generation
- Video Generation
- Text-to-Speech
- Embeddings
- Privacy
- OpenAI-Compatible
- x402
---
