---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 29
api_specs:
- filename: loops-api-key-api-openapi.yml
  format: yaml
  label: Loops API key API
  slug: loops-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-api-key-api-openapi.yml
- filename: loops-audience-segments-api-openapi.yml
  format: yaml
  label: Loops Audience segments API
  slug: loops-audience-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-audience-segments-api-openapi.yml
- filename: loops-campaign-groups-api-openapi.yml
  format: yaml
  label: Loops Campaign groups API
  slug: loops-campaign-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-campaign-groups-api-openapi.yml
- filename: loops-campaigns-api-openapi.yml
  format: yaml
  label: Loops Campaigns API
  slug: loops-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-campaigns-api-openapi.yml
- filename: loops-components-api-openapi.yml
  format: yaml
  label: Loops Components API
  slug: loops-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-components-api-openapi.yml
- filename: loops-configuration-api-openapi.yml
  format: yaml
  label: Loops Configuration API
  slug: loops-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-configuration-api-openapi.yml
- filename: loops-contact-properties-api-openapi.yml
  format: yaml
  label: Loops Contact properties API
  slug: loops-contact-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contact-properties-api-openapi.yml
- filename: loops-contacts-api-openapi.yml
  format: yaml
  label: Loops Contacts API
  slug: loops-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contacts-api-openapi.yml
- filename: loops-email-messages-api-openapi.yml
  format: yaml
  label: Loops Email messages API
  slug: loops-email-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-email-messages-api-openapi.yml
- filename: loops-event-patterns-api-openapi.yml
  format: yaml
  label: Loops Event patterns API
  slug: loops-event-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-event-patterns-api-openapi.yml
- filename: loops-events-api-openapi.yml
  format: yaml
  label: Loops Events API
  slug: loops-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-events-api-openapi.yml
- filename: loops-mailing-lists-api-openapi.yml
  format: yaml
  label: Loops Mailing lists API
  slug: loops-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-mailing-lists-api-openapi.yml
- filename: loops-themes-api-openapi.yml
  format: yaml
  label: Loops Themes API
  slug: loops-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-themes-api-openapi.yml
- filename: loops-transactional-emails-api-openapi.yml
  format: yaml
  label: Loops Transactional emails API
  slug: loops-transactional-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-transactional-emails-api-openapi.yml
- filename: loops-transactional-groups-api-openapi.yml
  format: yaml
  label: Loops Transactional groups API
  slug: loops-transactional-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-transactional-groups-api-openapi.yml
- filename: loops-uploads-api-openapi.yml
  format: yaml
  label: Loops Uploads API
  slug: loops-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-uploads-api-openapi.yml
- filename: loops-workflow-nodes-api-openapi.yml
  format: yaml
  label: Loops Workflow nodes API
  slug: loops-workflow-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-workflow-nodes-api-openapi.yml
- filename: loops-workflows-api-openapi.yml
  format: yaml
  label: Loops Workflows API
  slug: loops-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-workflows-api-openapi.yml
- filename: loops-webhooks-asyncapi.yml
  format: yaml
  label: Loops Webhooks
  slug: loops-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/asyncapi/loops-webhooks-asyncapi.yml
- filename: loops-webhooks-api-openapi.yml
  format: yaml
  label: Loops Webhooks API
  slug: loops-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-webhooks-api-openapi.yml
consequence_counts:
  physical: 3
  read: 29
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Loops Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/email-messages/{emailMessageId}/preview
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/events/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactional
operation_count: 64
overview: 'Loops exposes 64 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 32 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Loops
provider_slug: loops
slug: loops-agentic-access
source_filename: loops-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/loops-api-key-api-openapi.yml, openapi/loops-audience-segments-api-openapi.yml,\n  openapi/loops-campaign-groups-api-openapi.yml, openapi/loops-campaigns-api-openapi.yml, openapi/loops-components-api-openapi.yml,\n  openapi/loops-configuration-api-openapi.yml, openapi/loops-contact-properties-api-openapi.yml,\n  openapi/loops-contacts-api-openapi.yml, openapi/loops-email-messages-api-openapi.yml, openapi/loops-event-patterns-api-openapi.yml,\n  openapi/loops-events-api-openapi.yml, openapi/loops-mailing-lists-api-openapi.yml, openapi/loops-themes-api-openapi.yml,\n  openapi/loops-transactional-emails-api-openapi.yml, openapi/loops-transactional-groups-api-openapi.yml,\n  openapi/loops-uploads-api-openapi.yml, openapi/loops-workflow-nodes-api-openapi.yml, openapi/loops-workflows-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance\
  \ starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 64\n  by_action_class:\n    connected: 29\n    acting: 35\n  by_consequence:\n    read: 29\n    write: 32\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/api-key\n  method: get\n  operationId: testApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audience-segments/{audienceSegmentId}\n  method: get\n  operationId: getAudienceSegment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audience-segments\n  method: get\n  operationId: listAudienceSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/audience-segments\n  method: post\n  operationId: createAudienceSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaign-groups\n  method: get\n  operationId: listCampaignGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaign-groups\n  method: post\n  operationId: createCampaignGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaign-groups/{campaignGroupId}\n\
  \  method: get\n  operationId: getCampaignGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaign-groups/{campaignGroupId}\n  method: post\n  operationId: updateCampaignGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns/{campaignId}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{campaignId}\n  method: post\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components/{componentId}\n  method: get\n  operationId: getComponent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/components/{componentId}\n  method: post\n\
  \  operationId: updateComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/components\n  method: get\n  operationId: listComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/components\n  method: post\n  operationId: createComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dedicated-sending-ips\n  method: get\n  operationId: listDedicatedSendingIps\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/properties\n  method: post\n  operationId: createContactProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/properties\n  method: get\n  operationId: listContactProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/create\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/update\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/find\n  method: get\n  operationId: findContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/delete\n  method: post\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/suppression\n\
  \  method: get\n  operationId: getContactSuppression\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/suppression\n  method: delete\n  operationId: removeContactSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email-messages/{emailMessageId}\n  method: get\n  operationId: getEmailMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email-messages/{emailMessageId}\n  method: post\n  operationId: updateEmailMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email-messages/{emailMessageId}/preview\n  method: post\n  operationId: previewEmailMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email-messages/{emailMessageId}/guardian\n  method: get\n  operationId: getEmailMessageGuardian\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/event-patterns\n  method: get\n  operationId: listEventPatterns\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/event-patterns/by-name/{eventName}\n  method: get\n  operationId: getEventPatternByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/event-patterns/{eventPatternId}\n  method: get\n  operationId: getEventPattern\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/send\n  method: post\n  operationId: sendEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists\n\
  \  method: get\n  operationId: listMailingLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/themes/{themeId}\n  method: get\n  operationId: getTheme\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/themes/{themeId}\n  method: post\n  operationId: updateTheme\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/themes\n  method: get\n  operationId: listThemes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/themes\n  method:\
  \ post\n  operationId: createTheme\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactional\n  method: post\n  operationId: sendTransactionalEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactional\n  method: get\n  operationId: listPublishedTransactionalEmails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactional-emails\n \
  \ method: get\n  operationId: listTransactionalEmails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactional-emails\n  method: post\n  operationId: createTransactionalEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactional-emails/{transactionalId}\n  method: get\n  operationId: getTransactionalEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactional-emails/{transactionalId}\n  method: post\n  operationId: updateTransactionalEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactional-emails/{transactionalId}/draft\n  method: post\n  operationId: ensureTransactionalDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactional-emails/{transactionalId}/publish\n  method: post\n  operationId: publishTransactionalEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/transactional-groups\n  method: get\n  operationId: listTransactionalGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactional-groups\n  method: post\n  operationId: createTransactionalGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactional-groups/{transactionalGroupId}\n  method: get\n  operationId: getTransactionalGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactional-groups/{transactionalGroupId}\n  method: post\n  operationId: updateTransactionalGroup\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/{emailAssetId}/complete\n  method: post\n  operationId: completeUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{workflowId}/nodes\n  method:\
  \ post\n  operationId: createWorkflowNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{workflowId}/nodes/{nodeId}/add-branch\n  method: post\n  operationId: addWorkflowBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{workflowId}/nodes/{nodeId}\n  method: get\n  operationId: getWorkflowNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflows/{workflowId}/nodes/{nodeId}\n\
  \  method: post\n  operationId: updateWorkflowNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{workflowId}/nodes/{nodeId}\n  method: delete\n  operationId: deleteWorkflowNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{workflowId}/nodes/{nodeId}/reroute\n  method: post\n  operationId: rerouteNodeConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{workflowId}/nodes/{nodeId}/recursive\n  method: delete\n  operationId: deleteWorkflowNodeRecursively\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflows\n  method: post\n  operationId: createWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{workflowId}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflows/{workflowId}\n  method: post\n  operationId: updateWorkflowProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows/{workflowId}/mailing-list\n  method: post\n  operationId: changeWorkflowMailingList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/agentic-access/loops-agentic-access.yml
summary_line: 64 operations · 35 acting
tags:
- Email
- Email API
- Marketing Automation
- Transactional Email
- Lifecycle Email
- Webhook
- Software-as-a-Service
- Communications
- Developer Tools
- MCP
- Agents
- Campaigns
---
