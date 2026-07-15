---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: ariba-sourcing-external-approval-api.yaml
  format: yaml
  label: Ariba Sourcing - External Approval API
  slug: ariba-sourcing-external-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/openapi/ariba-sourcing-external-approval-api.yaml
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ariba Sourcing Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Ariba Sourcing exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
slug: ariba-sourcing-agentic-access
source_filename: ariba-sourcing-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ariba-sourcing-external-approval-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /changes\n  method: get\n  operationId: listApprovalChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pendingApprovables\n  method: get\n  operationId: listPendingApprovables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /task/{entity_id}\n\
  \  method: get\n  operationId: getApprovalTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{entity_type}/{entity_id}\n  method: get\n  operationId: getApprovableDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action\n  method: post\n  operationId: submitApprovalAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Document/{documentId}/attachments/{docAttachmentId}\n  method: get\n  operationId: downloadAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/members\n  method: get\n  operationId: listGroupMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/agentic-access/ariba-sourcing-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Approvals
- Auctions
- B2B
- Contracts
- Procurement
- RFx
- SAP
- Sourcing
- Supplier Management
- Supply Chain
---
