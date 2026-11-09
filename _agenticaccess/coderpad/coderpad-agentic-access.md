---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 29
api_specs:
- filename: coderpad-account-api-openapi.yml
  format: yaml
  label: CoderPad Account API
  slug: coderpad-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-account-api-openapi.yml
- filename: coderpad-campaigns-api-openapi.yml
  format: yaml
  label: CoderPad Campaigns API
  slug: coderpad-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-campaigns-api-openapi.yml
- filename: coderpad-me-api-openapi.yml
  format: yaml
  label: CoderPad Me API
  slug: coderpad-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-me-api-openapi.yml
- filename: coderpad-organization-api-openapi.yml
  format: yaml
  label: CoderPad Organization API
  slug: coderpad-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-organization-api-openapi.yml
- filename: coderpad-pad-environments-api-openapi.yml
  format: yaml
  label: CoderPad Pad environments API
  slug: coderpad-pad-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-pad-environments-api-openapi.yml
- filename: coderpad-pads-api-openapi.yml
  format: yaml
  label: CoderPad Pads API
  slug: coderpad-pads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-pads-api-openapi.yml
- filename: coderpad-question-variants-api-openapi.yml
  format: yaml
  label: CoderPad Question variants API
  slug: coderpad-question-variants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-question-variants-api-openapi.yml
- filename: coderpad-questions-api-openapi.yml
  format: yaml
  label: CoderPad Questions API
  slug: coderpad-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-questions-api-openapi.yml
- filename: coderpad-temporaryfile-api-openapi.yml
  format: yaml
  label: CoderPad Temporary File API
  slug: coderpad-temporaryfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-temporaryfile-api-openapi.yml
- filename: coderpad-tests-api-openapi.yml
  format: yaml
  label: CoderPad Tests API
  slug: coderpad-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-tests-api-openapi.yml
- filename: coderpad-webhook-api-openapi.yml
  format: yaml
  label: CoderPad Webhook API
  slug: coderpad-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderpad/openapi/coderpad-webhook-api-openapi.yml
consequence_counts:
  physical: 2
  read: 29
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coderpad Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1.1/campaigns/{campaign_id}/actions/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1.1/tests/{id}/actions/resend
operation_count: 47
overview: 'CoderPad exposes 47 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 16 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CoderPad
provider_slug: coderpad
slug: coderpad-agentic-access
source_filename: coderpad-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/coderpad-interview-api-openapi.yml, openapi/coderpad-screen-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 29\n    acting: 18\n  by_consequence:\n    read: 29\n    write: 16\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /organization\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/pads\n  method: get\n  operationId: listOrganizationPads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /organization/questions\n  method: get\n  operationId: listOrganizationQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/stats\n  method: get\n  operationId: getOrganizationStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/users\n  method: get\n  operationId: listOrganizationUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pad_environments/{id}\n  method: get\n  operationId: getPadEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pads\n  method: get\n  operationId:\
  \ listPads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pads\n  method: post\n  operationId: createPad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pads/{id}\n  method: get\n  operationId: getPad\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pads/{id}\n  method: put\n  operationId: updatePad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /pads/{id}/events\n  method: get\n  operationId: listPadEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /questions\n  method: get\n  operationId: listQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /questions\n  method: post\n  operationId: createQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /questions/{id}\n  method: get\n  operationId: getQuestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /questions/{id}\n  method: put\n  operationId: updateQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /questions/{id}\n  method: delete\n  operationId: deleteQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /questions/{question_id}/variants\n  method: get\n  operationId: listQuestionVariants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /questions/{question_id}/variants\n\
  \  method: post\n  operationId: createQuestionVariant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /questions/{question_id}/variants/{id}\n  method: get\n  operationId: getQuestionVariant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /questions/{question_id}/variants/{id}\n  method: put\n  operationId: updateQuestionVariant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /questions/{question_id}/variants/{id}\n\
  \  method: delete\n  operationId: deleteQuestionVariant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quota\n  method: get\n  operationId: getQuota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/campaigns\n  method: get\n  operationId: campaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/campaigns\n  method: post\n  operationId:\
  \ createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/campaigns/{campaign_id}\n  method: get\n  operationId: campaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/campaigns/{campaign_id}/actions/send\n  method: post\n  operationId: send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/campaigns/{campaign_id}/insights\n  method: get\n\
  \  operationId: campaignInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/me\n  method: get\n  operationId: me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/questions\n  method: get\n  operationId: questions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/questions\n  method: post\n  operationId: createQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/questions/{id}\n  method: get\n  operationId: question\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/questions/{id}\n  method: put\n  operationId: updateQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/questions/{id}/insights\n  method: get\n  operationId: questionInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/temporary-file\n  method: post\n  operationId: upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/tests\n  method: get\n  operationId: testsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/tests/{id}\n  method: get\n  operationId: testStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/tests/{id}\n  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/tests/{id}/actions/cancel\n  method: post\n  operationId: cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/tests/{id}/actions/resend\n  method: post\n  operationId: resend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/tests/{id}/questions/{questionId}/ai-assist-conversations\n  method: get\n  operationId: aiAssistConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/tests/{id}/questions/{questionId}/playback-events\n  method: get\n  operationId: playbackEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/tests/{id}/questions/{questionId}/project\n  method: get\n  operationId: candidateProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/tests/{id}/report\n  method: get\n  operationId: report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/webhook\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/webhook\n  method: post\n  operationId: subscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.1/webhook\n  method: delete\n  operationId: unsubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/coderpad/agentic-access/coderpad-agentic-access.yml
summary_line: 47 operations · 18 acting
tags:
- Company
- Artificial Intelligence
- Hiring
- Technical Assessment
- InterviewPlatform
---
