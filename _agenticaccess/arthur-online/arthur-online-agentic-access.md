---
acting_count: 137
action_class_counts:
  acting: 137
  connected: 180
api_specs:
- filename: arthur-online-properties-openapi.yml
  format: yaml
  label: Arthur Properties API
  slug: arthur-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-properties-openapi.yml
- filename: arthur-online-units-openapi.yml
  format: yaml
  label: Arthur Units API
  slug: arthur-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-units-openapi.yml
- filename: arthur-online-tenancies-openapi.yml
  format: yaml
  label: Arthur Tenancies API
  slug: arthur-tenancies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-tenancies-openapi.yml
- filename: arthur-online-tenants-openapi.yml
  format: yaml
  label: Arthur Tenants API
  slug: arthur-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-tenants-openapi.yml
- filename: arthur-online-applicants-openapi.yml
  format: yaml
  label: Arthur Applicants API
  slug: arthur-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-applicants-openapi.yml
- filename: arthur-online-viewings-openapi.yml
  format: yaml
  label: Arthur Viewings API
  slug: arthur-viewings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-viewings-openapi.yml
- filename: arthur-online-maintenance-openapi.yml
  format: yaml
  label: Arthur Maintenance API
  slug: arthur-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-maintenance-openapi.yml
- filename: arthur-online-financials-openapi.yml
  format: yaml
  label: Arthur Financials API
  slug: arthur-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-financials-openapi.yml
- filename: arthur-online-assets-openapi.yml
  format: yaml
  label: Arthur Assets API
  slug: arthur-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-assets-openapi.yml
- filename: arthur-online-utilities-openapi.yml
  format: yaml
  label: Arthur Utilities API
  slug: arthur-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-utilities-openapi.yml
- filename: arthur-online-certificates-openapi.yml
  format: yaml
  label: Arthur Certificates API
  slug: arthur-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-certificates-openapi.yml
- filename: arthur-online-entities-openapi.yml
  format: yaml
  label: Arthur Entities API
  slug: arthur-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-entities-openapi.yml
- filename: arthur-online-conversations-openapi.yml
  format: yaml
  label: Arthur Conversations API
  slug: arthur-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-conversations-openapi.yml
- filename: arthur-online-tags-openapi.yml
  format: yaml
  label: Arthur Tags API
  slug: arthur-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-tags-openapi.yml
- filename: arthur-online-notes-openapi.yml
  format: yaml
  label: Arthur Notes API
  slug: arthur-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-notes-openapi.yml
- filename: arthur-online-types-openapi.yml
  format: yaml
  label: Arthur Types API
  slug: arthur-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/openapi/arthur-online-types-openapi.yml
consequence_counts:
  physical: 19
  read: 180
  write: 118
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Arthur Online Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /properties/{property_id}/workorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /properties/{property_id}/workorders/{workorder_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tasks/{task_id}/workorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /tasks/{task_id}/workorders/{workorder_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /tenancies/{id}/register_deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tenancies/{tenancy_id}/workorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /tenancy/{tenancy_id}/workorders/{workorder_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /units/{unit_id}/workorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /units/{unit_id}/workorders/{workorder_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /workorders/{workorder_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workorders/{workorder_id}/assets
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /workorders/{workorder_id}/contractors/{contractor_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workorders/{workorder_id}/conversations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workorders/{workorder_id}/notes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /workorders/{workorder_id}/notes/{note_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /workorders/{workorder_id}/notes/{note_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /workorders/{workorder_id}/tags
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /workorders/{workorder_id}/untag
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /workorders/{workorder_id}/untag_all
operation_count: 317
overview: 'Arthur Online exposes 317 API operations that an AI agent could call, of which 137 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 180 read, 118 write, and 19 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Arthur Online
provider_slug: arthur-online
slug: arthur-online-agentic-access
source_filename: arthur-online-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/arthur-online-applicants-openapi.yml, openapi/arthur-online-assets-openapi.yml,\n  openapi/arthur-online-certificates-openapi.yml, openapi/arthur-online-conversations-openapi.yml,\n  openapi/arthur-online-entities-openapi.yml, openapi/arthur-online-financials-openapi.yml,\n  openapi/arthur-online-maintenance-openapi.yml, openapi/arthur-online-notes-openapi.yml, openapi/arthur-online-properties-openapi.yml,\n  openapi/arthur-online-tags-openapi.yml, openapi/arthur-online-tenancies-openapi.yml, openapi/arthur-online-tenants-openapi.yml,\n  openapi/arthur-online-types-openapi.yml, openapi/arthur-online-units-openapi.yml, openapi/arthur-online-utilities-openapi.yml,\n  openapi/arthur-online-viewings-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment.\
  \ See research/curity/agentic-governance/.\nsummary:\n  operations: 317\n  by_action_class:\n    connected: 180\n    acting: 137\n  by_consequence:\n    read: 180\n    write: 118\n    physical: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /applicants/{applicant_id}/assets\n  method: get\n  operationId: listAssetsOnApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}/assets\n  method: post\n  operationId: createAssetOnApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}/managers/{manager_id}\n  method: get\n  operationId: listManagersOnApplicant\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}/managers/{manager_id}\n  method: delete\n  operationId: deleteManagerOnApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}/managers\n  method: post\n  operationId: addManagerOnApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}/credit_checks\n  method: get\n  operationId: listCreditChecksOnApplicant\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}/conversation_recipients\n  method: get\n  operationId: getRecipientsForApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}/conversations\n  method: get\n  operationId: listConversationsOnApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}/conversations\n  method: post\n  operationId: createConversationOnApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /applicants/{applicant_id}/viewings\n  method: get\n  operationId: listViewingsOnApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}/viewings\n  method: post\n  operationId: addViewingOnApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}/notes\n  method: get\n  operationId: listNotesOnApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}/notes\n  method: post\n  operationId: addNoteOnApplicant\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}/notes/{note_id}\n  method: get\n  operationId: viewNoteOnApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}/notes/{note_id}\n  method: put\n  operationId: updateNoteOnApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}/notes/{note_id}\n  method: delete\n  operationId: deleteNoteOnApplicant\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}/tags\n  method: get\n  operationId: listTagsOnApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}/tags\n  method: put\n  operationId: tagApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}/untag\n  method: put\n  operationId: untagApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}/untag_all\n  method: put\n  operationId: untagAllApplicantTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants\n  method: get\n  operationId: listApplicants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants\n  method: post\n  operationId: addApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{applicant_id}\n  method: get\n  operationId: viewApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{applicant_id}\n  method: put\n  operationId: updateApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicant/{applicant_id}/status\n  method: put\n  operationId: updateApplicantStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets\n  method: post\n  operationId: createAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{asset_id}\n  method: get\n  operationId: viewAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{asset_id}\n  method: put\n  operationId: updateAsset\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{asset_id}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /certificates\n  method: get\n  operationId: listCertificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /certificates/{certificate_id}\n  method: get\n  operationId: viewCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /certificates/{certificate_id}\n  method: put\n  operationId: updateCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /certificates/{certificate_id}\n  method: delete\n  operationId: deleteCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/assets\n  method: get\n  operationId: listAssetsOnConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /conversations/{conversation_id}/messages\n  method: get\n  operationId: listMessagesRelatedToConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/messages\n  method: post\n  operationId: addMessagesRelatedToConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/messages/{message_id}\n  method: get\n  operationId: viewMessageRelatedToConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}\n  method: get\n  operationId:\
  \ listConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities\n  method: get\n  operationId: listEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities\n  method: post\n  operationId: createEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entities/{entity_id}\n  method: get\n  operationId: viewEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/{entity_id}\n  method: put\n  operationId: updateEntity\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entities/{entity_id}\n  method: delete\n  operationId: deleteEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurrings/{recurringId}\n  method: get\n  operationId: viewRecurring\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_id}\n  method: get\n  operationId: viewTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_id}/payoff\n  method: put\n  operationId: payoffTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoice_id}\n  method: get\n  operationId: viewInvoices\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/subtasks\n  method: get\n  operationId: listSubtasksOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/subtasks\n  method: post\n  operationId: createSubtaskOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/subtasks/{subtask_id}\n  method: get\n  operationId: viewSubtaskOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/subtasks/{subtask_id}\n  method:\
  \ put\n  operationId: updateSubtaskOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/subtasks/{subtask_id}\n  method: delete\n  operationId: deleteSubtaskOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/workorders\n  method: get\n  operationId: listWorkordersOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/workorders\n  method: post\n  operationId:\
  \ createWorkorderOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/workorders/{workorder_id}\n  method: get\n  operationId: viewWorkorderOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/workorders/{workorder_id}\n  method: put\n  operationId: updateWorkorderOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /tasks/{task_id}/tags\n  method: get\n  operationId: listTagsOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/tags\n  method: put\n  operationId: tagTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/untag\n  method: put\n  operationId: untagTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/untag_all\n \
  \ method: put\n  operationId: untagAllTaskTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/notes\n  method: get\n  operationId: listNotesOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/notes\n  method: post\n  operationId: createNoteOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/notes/{note_id}\n  method: get\n  operationId: viewNoteOnTask\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/notes/{note_id}\n  method: put\n  operationId: updateNoteOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/notes/{note_id}\n  method: delete\n  operationId: deleteNoteOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/conversation_recipients\n  method: get\n  operationId: getRecipientsForTask\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/conversations\n  method: get\n  operationId: listConversationsOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/conversations\n  method: post\n  operationId: addConversationOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/assets\n  method: get\n  operationId: listAssetsOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/assets/{asset_id}\n  method:\
  \ get\n  operationId: viewAssetOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/tenants\n  method: get\n  operationId: listTenantsOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/tenants/{tenant_id}\n  method: get\n  operationId: viewTenantOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{status}\n  method: get\n  operationId: listTasksByStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}\n  method: get\n  operationId: viewTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}\n  method: put\n  operationId: updateTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}\n  method: delete\n  operationId: deleteTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/status\n\
  \  method: put\n  operationId: updateStatusOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subtasks\n  method: get\n  operationId: listSubtasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subtasks/{subtask_id}\n  method: get\n  operationId: viewSubtask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subtasks/{subtask_id}\n  method: put\n  operationId: updateSubtask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subtasks/{subtask_id}\n  method: delete\n  operationId: deleteSubtask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workorders/{workorder_id}/transactions\n  method: get\n  operationId: listTransactionsOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/certificates\n  method: get\n  operationId: listCertificatesOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/quotes\n\
  \  method: get\n  operationId: listQuotesOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/quotes/{quote_id}\n  method: get\n  operationId: viewQuoteOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/invoices\n  method: get\n  operationId: listInvoicesOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/invoices/{invoice_id}\n  method: get\n  operationId: viewInvoiceOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/assets\n\
  \  method: get\n  operationId: listAssetsOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/assets\n  method: post\n  operationId: createAssetOnWorkorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workorders/{workorder_id}/assets/{edge_id}\n  method: get\n  operationId: viewAssetOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/conversation_recipients\n  method: get\n  operationId: getRecipientsForWorkorder\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/conversations\n  method: get\n  operationId: listConversationsOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/conversations\n  method: post\n  operationId: createConversationOnWorkorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workorders/{workorder_id}/notes\n  method: get\n  operationId: listNotesOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/notes\n  method: post\n  operationId: addNoteOnWorkorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workorders/{workorder_id}/notes/{edge_id}\n  method: get\n  operationId: viewNoteOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/notes/{note_id}\n  method: put\n  operationId: updateNoteOnWorkorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workorders/{workorder_id}/notes/{note_id}\n  method: delete\n  operationId: deleteNoteOnWorkorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workorders/{workorder_id}/tags\n  method: get\n  operationId: listTagsOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/tags\n  method: put\n  operationId: tagWorkorder\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workorders/{workorder_id}/untag\n  method: put\n  operationId: untagWorkorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workorders/{workorder_id}/untag_all\n  method: put\n  operationId: untagAllWorkorderTags\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workorders/{workorder_id}/contractors\n  method: get\n  operationId: listContractorsOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/contractors/{contractor_id}\n  method: get\n  operationId: viewContractorOnWorkorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workorders/{workorder_id}/contractors/{contractor_id}\n  method: delete\n  operationId: deleteContractorOnWorkorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-v\n\n# --- truncated at 32 KB (88 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/agentic-access/arthur-online-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthur-online/refs/heads/main/agentic-access/arthur-online-agentic-access.yml
summary_line: 317 operations · 137 acting
tags:
- Real-Estate
- United Kingdom
- Property Management
- PropTech
- Rentals
- Lettings
- Tenancy
- Maintenance
- Property Listings
- Social Housing
- Student Housing
- Block Management
---
