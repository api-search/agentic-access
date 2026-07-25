---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 25
api_specs:
- filename: pandadoc-api-logs-api-openapi.yml
  format: yaml
  label: PandaDoc API Logs API
  slug: pandadoc-api-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-api-logs-api-openapi.yml
- filename: pandadoc-contacts-api-openapi.yml
  format: yaml
  label: PandaDoc Contacts API
  slug: pandadoc-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-contacts-api-openapi.yml
- filename: pandadoc-document-attachments-api-openapi.yml
  format: yaml
  label: PandaDoc Document Attachments API
  slug: pandadoc-document-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-attachments-api-openapi.yml
- filename: pandadoc-document-fields-api-openapi.yml
  format: yaml
  label: PandaDoc Document Fields API
  slug: pandadoc-document-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-fields-api-openapi.yml
- filename: pandadoc-document-link-to-crm-api-openapi.yml
  format: yaml
  label: PandaDoc Document Link to CRM API
  slug: pandadoc-document-link-to-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-link-to-crm-api-openapi.yml
- filename: pandadoc-document-recipients-api-openapi.yml
  format: yaml
  label: PandaDoc Document Recipients API
  slug: pandadoc-document-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-recipients-api-openapi.yml
- filename: pandadoc-document-reminders-api-openapi.yml
  format: yaml
  label: PandaDoc Document Reminders API
  slug: pandadoc-document-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-reminders-api-openapi.yml
- filename: pandadoc-documents-api-openapi.yml
  format: yaml
  label: PandaDoc Documents API
  slug: pandadoc-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-documents-api-openapi.yml
- filename: pandadoc-folders-api-openapi.yml
  format: yaml
  label: PandaDoc Folders API
  slug: pandadoc-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-folders-api-openapi.yml
- filename: pandadoc-forms-api-openapi.yml
  format: yaml
  label: PandaDoc Forms API
  slug: pandadoc-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-forms-api-openapi.yml
- filename: pandadoc-members-api-openapi.yml
  format: yaml
  label: PandaDoc Members API
  slug: pandadoc-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-members-api-openapi.yml
- filename: pandadoc-templates-api-openapi.yml
  format: yaml
  label: PandaDoc Templates API
  slug: pandadoc-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-templates-api-openapi.yml
- filename: pandadoc-webhook-events-api-openapi.yml
  format: yaml
  label: PandaDoc Webhook Events API
  slug: pandadoc-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-webhook-events-api-openapi.yml
- filename: pandadoc-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: PandaDoc Webhook Subscriptions API
  slug: pandadoc-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-webhook-subscriptions-api-openapi.yml
- filename: pandadoc-workspaces-api-openapi.yml
  format: yaml
  label: PandaDoc Workspaces API
  slug: pandadoc-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-workspaces-api-openapi.yml
consequence_counts:
  physical: 1
  read: 25
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pandadoc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /documents/{id}/send
operation_count: 43
overview: 'PandaDoc exposes 43 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 17 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PandaDoc
provider_slug: pandadoc
slug: pandadoc-agentic-access
source_filename: pandadoc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pandadoc-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 25\n    acting: 18\n  by_consequence:\n    read: 25\n    write: 17\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}\n  method: get\n  operationId: getDocumentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/status\n  method: get\n  operationId: getDocumentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}/send\n  method: post\n  operationId: sendDocument\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/download\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}/session\n  method: post\n  operationId: createDocumentSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/recipients\n  method: get\n  operationId: listDocumentRecipients\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}/recipients\n  method: post\n  operationId: addDocumentRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/recipients/{recipient_id}\n  method: patch\n  operationId: updateDocumentRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/recipients/{recipient_id}\n  method: delete\n  operationId: deleteDocumentRecipient\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/fields\n  method: get\n  operationId: listDocumentFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}/fields\n  method: patch\n  operationId: updateDocumentFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/attachments\n  method: get\n  operationId: listDocumentAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}/attachments/{attachment_id}/download\n  method: get\n  operationId: downloadDocumentAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/auto-reminders\n  method: get\n  operationId: getDocumentAutoReminders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/linked-objects\n  method: get\n  operationId: listLinkedObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /templates/{id}/details\n  method: get\n  operationId: getTemplateDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/{id}\n  method: delete\n  operationId: deleteTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /forms\n  method: get\n  operationId: listForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/folders\n  method: get\n  operationId: listDocumentFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/folders\n  method: post\n  operationId: createDocumentFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: get\n  operationId:\
  \ getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/current\n  method: get\n  operationId: getCurrentMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/{id}\n  method: get\n  operationId: getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-subscriptions\n  method: get\n  operationId: listWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions/{id}\n  method: get\n  operationId: getWebhookSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-subscriptions/{id}\n  method: patch\n  operationId: updateWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions/{id}\n  method: delete\n  operationId: deleteWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions/{id}/shared-key\n  method: patch\n  operationId: updateWebhookSubscriptionSharedKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-events\n  method: get\n  operationId: listWebhookEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-events/{id}\n  method: get\n  operationId: getWebhookEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs\n  method: get\n  operationId: listApiLogs\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/agentic-access/pandadoc-agentic-access.yml
summary_line: 43 operations · 18 acting
tags:
- Document Automation
- E-Signature
- Document Management
- Document Generation
- Webhooks
---
