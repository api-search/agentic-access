---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 17
api_specs:
- filename: novelai-openapi.yml
  format: yaml
  label: NovelAI API
  slug: novelai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/openapi/novelai-openapi.yml
consequence_counts:
  read: 17
  safety-critical: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 35
kind: agentic-access
layout: agentic-access
method: generated
name: Novelai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/annotate-image
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/classify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/generate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/generate-image
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/generate-prompt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/generate-stream
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/generate-voice
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/module/buy-training-steps
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ai/module/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai/upscale
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/change-access-key
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /user/change-mailing-list-consent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /user/clientsettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /user/consent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/create-persistent-token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/deletion/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/deletion/request
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /user/keystore
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/login
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /user/objects/batch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /user/objects/{type}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /user/objects/{type}/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /user/objects/{type}/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/recovery/recover
operation_count: 52
overview: 'NovelAI exposes 52 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 35 safety-critical.


  35 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NovelAI
provider_slug: novelai
slug: novelai-agentic-access
source_filename: novelai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/novelai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 17\n    acting: 35\n  by_consequence:\n    read: 17\n    safety-critical: 35\n  human_in_the_loop_required: 35\noperations:\n- path: /\n  method: get\n  operationId: AppController_healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/register\n  method: post\n  operationId: UserController_createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/login\n  method: post\n  operationId: UserController_loginUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/change-access-key\n  method: post\n  operationId: UserController_changeAccessKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/sso/google\n  method: post\n  operationId:\
  \ UserController_ssoGoogle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/change-mailing-list-consent\n  method: patch\n  operationId: UserController_changeMailingListConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/resend-email-verification\n  method: post\n  operationId: UserController_requestEmailVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/verify-email\n  method: post\n  operationId: UserController_verifyEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/information\n  method: get\n  operationId: UserController_getAccountInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/osano-external-id\n  method: get\n  operationId: UserController_getOsanoExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/consent\n  method: put\n  operationId: UserController_upsertUserConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/deletion/request\n  method: post\n  operationId: UserController_requestAccountDeletion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/deletion/delete\n  method: post\n  operationId: UserController_deleteAccount\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/recovery/request\n  method: post\n  operationId: UserController_requestAccountRecovery\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/recovery/recover\n  method: post\n  operationId: UserController_recoverAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/delete\n  method: post\n  operationId: UserController_deleteAccountUnchecked\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/data\n  method: get\n  operationId: UserController_getUserData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/priority\n  method: get\n  operationId: UserController_getCurrentPriority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/giftkeys\n\
  \  method: get\n  operationId: UserController_getGiftKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/subscription\n  method: get\n  operationId: UserController_getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/keystore\n  method: get\n  operationId: UserController_getKeystore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/keystore\n  method: put\n  operationId: UserController_updateKeystore\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /user/objects/{type}\n  method: get\n  operationId: UserController_getObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/objects/{type}\n  method: put\n  operationId: UserController_createObject\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/objects/{type}/{id}\n  method: get\n  operationId: UserController_getObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/objects/{type}/{id}\n  method: patch\n  operationId: UserController_editObject\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/objects/{type}/{id}\n  method: delete\n  operationId: UserController_deleteObject\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/clientsettings\n  method: get\n  operationId: UserController_getClientSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/clientsettings\n  method:\
  \ put\n  operationId: UserController_updateClientSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/objects/batch\n  method: delete\n  operationId: UserController_batchDeleteObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/create-persistent-token\n  method: post\n  operationId: UserController_createPersistentToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/submission\n  method: post\n  operationId: UserController_postUserSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/submission/{event}\n  method: get\n  operationId: UserController_getUserSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/vote-submission/{event}\n  method: get\n  operationId: UserController_getUserSubmissionVotes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/vote-submission/{event}\n  method: post\n  operationId: UserController_voteSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/vote-submission/{event}\n  method: delete\n  operationId: UserController_retractSubmissionVote\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/subscription/bind\n  method: post\n  operationId:\
  \ SubscriptionController_bindSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/subscription/change\n  method: post\n  operationId: SubscriptionController_changeSubscriptionPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/generate\n  method: post\n  operationId: AIController_aiGenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/generate-prompt\n  method: post\n  operationId: AIController_aiGeneratePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/generate-stream\n  method: post\n  operationId: AIController_aiGenerateStreamable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /ai/annotate-image\n  method: post\n  operationId: AIController_annotateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/generate-image\n  method: post\n  operationId: AIController_aiGenerateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/upscale\n  method: post\n  operationId: AIController_aiUpscaleImage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/classify\n  method: post\n  operationId: AIController_classify\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/generate-image/suggest-tags\n  method: get\n  operationId: AIController_generateImageTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/generate-voice\n  method: get\n  operationId: AIController_generateVoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/generate-voice\n  method: post\n  operationId: AIController_generateVoicePost\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/module/all\n  method: get\n  operationId: AIModuleController_allModules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/module/{id}\n  method: get\n  operationId: AIModuleController_getModule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/module/{id}\n  method: delete\n  operationId: AIModuleController_deleteModule\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai/module/buy-training-steps\n  method: post\n  operationId: AIModuleController_buyTrainingSteps\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/agentic-access/novelai-agentic-access.yml
summary_line: 52 operations · 35 acting · 35 human-in-the-loop
tags:
- AI
- Image Generation
- LLM
- Storytelling
---
