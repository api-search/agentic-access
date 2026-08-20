---
acting_count: 112
action_class_counts:
  acting: 112
api_specs:
- filename: outline-accessrequests-api-openapi.yml
  format: yaml
  label: Outline AccessRequests API
  slug: outline-accessrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-accessrequests-api-openapi.yml
- filename: outline-attachments-api-openapi.yml
  format: yaml
  label: Outline Attachments API
  slug: outline-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-attachments-api-openapi.yml
- filename: outline-auth-api-openapi.yml
  format: yaml
  label: Outline Auth API
  slug: outline-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-auth-api-openapi.yml
- filename: outline-collections-api-openapi.yml
  format: yaml
  label: Outline Collections API
  slug: outline-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-collections-api-openapi.yml
- filename: outline-comments-api-openapi.yml
  format: yaml
  label: Outline Comments API
  slug: outline-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-comments-api-openapi.yml
- filename: outline-dataattributes-api-openapi.yml
  format: yaml
  label: Outline DataAttributes API
  slug: outline-dataattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-dataattributes-api-openapi.yml
- filename: outline-documents-api-openapi.yml
  format: yaml
  label: Outline Documents API
  slug: outline-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-documents-api-openapi.yml
- filename: outline-events-api-openapi.yml
  format: yaml
  label: Outline Events API
  slug: outline-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-events-api-openapi.yml
- filename: outline-fileoperations-api-openapi.yml
  format: yaml
  label: Outline FileOperations API
  slug: outline-fileoperations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-fileoperations-api-openapi.yml
- filename: outline-groups-api-openapi.yml
  format: yaml
  label: Outline Groups API
  slug: outline-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-groups-api-openapi.yml
- filename: outline-oauthauthentications-api-openapi.yml
  format: yaml
  label: Outline OAuthAuthentications API
  slug: outline-oauthauthentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-oauthauthentications-api-openapi.yml
- filename: outline-oauthclients-api-openapi.yml
  format: yaml
  label: Outline OAuthClients API
  slug: outline-oauthclients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-oauthclients-api-openapi.yml
- filename: outline-revisions-api-openapi.yml
  format: yaml
  label: Outline Revisions API
  slug: outline-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-revisions-api-openapi.yml
- filename: outline-shares-api-openapi.yml
  format: yaml
  label: Outline Shares API
  slug: outline-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-shares-api-openapi.yml
- filename: outline-stars-api-openapi.yml
  format: yaml
  label: Outline Stars API
  slug: outline-stars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-stars-api-openapi.yml
- filename: outline-templates-api-openapi.yml
  format: yaml
  label: Outline Templates API
  slug: outline-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-templates-api-openapi.yml
- filename: outline-users-api-openapi.yml
  format: yaml
  label: Outline Users API
  slug: outline-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-users-api-openapi.yml
- filename: outline-views-api-openapi.yml
  format: yaml
  label: Outline Views API
  slug: outline-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-views-api-openapi.yml
consequence_counts:
  physical: 6
  safety-critical: 1
  write: 105
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Outline Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /shares.revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collections.group_memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collections.memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /documents.group_memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /documents.memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /groups.memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stars.update
operation_count: 112
overview: 'Outline exposes 112 API operations that an AI agent could call, of which 112 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 105 write, 6 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Outline
provider_slug: outline
slug: outline-agentic-access
source_filename: outline-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/outline-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 112\n  by_action_class:\n    acting: 112\n  by_consequence:\n    write: 105\n    physical: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /accessRequests.create\n  method: post\n  operationId: accessRequestsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /accessRequests.info\n  method: post\n  operationId:\
  \ accessRequestsInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /accessRequests.approve\n  method: post\n  operationId: accessRequestsApprove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /accessRequests.dismiss\n  method: post\n  operationId: accessRequestsDismiss\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /attachments.create\n  method: post\n  operationId: attachmentsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /attachments.redirect\n  method: post\n  operationId: attachmentsRedirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /attachments.delete\n  method: post\n  operationId: attachmentsDelete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /auth.info\n  method: post\n  operationId: authInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /auth.config\n  method: post\n  operationId: authConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n    scope:\n    - read\n    - write\n- path: /collections.info\n  method: post\n  operationId: collectionsInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.documents\n  method: post\n  operationId: collectionsDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.list\n  method: post\n  operationId: collectionsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.create\n  method: post\n  operationId: collectionsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.update\n  method: post\n  operationId: collectionsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    -\
  \ write\n- path: /collections.add_user\n  method: post\n  operationId: collectionsAddUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.remove_user\n  method: post\n  operationId: collectionsRemoveUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.memberships\n  method: post\n  operationId: collectionsMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.add_group\n  method: post\n  operationId: collectionsAddGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.remove_group\n  method: post\n  operationId: collectionsRemoveGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.group_memberships\n  method: post\n  operationId: collectionsGroupMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.delete\n  method: post\n  operationId: collectionsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.export\n  method: post\n  operationId: collectionsExport\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /collections.export_all\n  method: post\n  operationId: collectionsExportAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /comments.create\n  method: post\n  operationId: commentsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /comments.info\n  method: post\n  operationId: commentsInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /comments.update\n  method: post\n  operationId: commentsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /comments.delete\n  method: post\n  operationId: commentsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /comments.list\n  method: post\n  operationId: commentsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /dataAttributes.info\n  method: post\n  operationId: dataAttributesInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - read\n    - write\n- path: /dataAttributes.list\n  method: post\n  operationId: dataAttributesList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /dataAttributes.create\n  method: post\n  operationId: dataAttributesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /dataAttributes.update\n  method: post\n  operationId: dataAttributesUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /dataAttributes.delete\n  method: post\n  operationId: dataAttributesDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.info\n  method: post\n  operationId: documentsInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n\
  - path: /documents.insights\n  method: post\n  operationId: documentsInsights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.import\n  method: post\n  operationId: documentsImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.export\n  method: post\n  operationId: documentsExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.list\n  method: post\n  operationId: documentsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.documents\n  method: post\n  operationId: documentsDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.drafts\n  method: post\n  operationId:\
  \ documentsDrafts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.viewed\n  method: post\n  operationId: documentsViewed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.answerQuestion\n  method: post\n  operationId: documentsAnswerQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.search_titles\n  method: post\n  operationId: documentsSearchTitles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.search\n  method: post\n  operationId: documentsSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.create\n  method: post\n  operationId: documentsCreate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.update\n  method: post\n  operationId: documentsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.templatize\n  method: post\n  operationId: documentsTemplatize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.unpublish\n  method: post\n  operationId: documentsUnpublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.move\n  method: post\n  operationId: documentsMove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.archive\n  method: post\n  operationId: documentsArchive\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.restore\n  method: post\n  operationId: documentsRestore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.delete\n  method: post\n  operationId: documentsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - read\n    - write\n- path: /documents.users\n  method: post\n  operationId: documentsUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.memberships\n  method: post\n  operationId: documentsMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.add_user\n  method: post\n  operationId: documentsAddUser\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.remove_user\n  method: post\n  operationId: documentsRemoveUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.archived\n  method: post\n  operationId: documentsArchived\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  \    scope:\n    - read\n    - write\n- path: /documents.deleted\n  method: post\n  operationId: documentsDeleted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.duplicate\n  method: post\n  operationId: documentsDuplicate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.add_group\n  method: post\n  operationId: documentsAddGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.remove_group\n  method: post\n  operationId: documentsRemoveGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.group_memberships\n  method: post\n  operationId: documentsGroupMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /documents.empty_trash\n  method: post\n  operationId: documentsEmptyTrash\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /events.list\n  method: post\n  operationId: eventsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /fileOperations.info\n  method: post\n  operationId: fileOperationsInfo\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /fileOperations.delete\n  method: post\n  operationId: fileOperationsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /fileOperations.redirect\n  method: post\n  operationId: fileOperationsRedirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n    scope:\n    - read\n    - write\n- path: /fileOperations.list\n  method: post\n  operationId: fileOperationsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /groups.info\n  method: post\n  operationId: groupsInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /groups.list\n  method: post\n  operationId: groupsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /groups.create\n  method: post\n  operationId: groupsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /groups.update\n  method: post\n  operationId: groupsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /groups.delete\n \
  \ method: post\n  operationId: groupsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /groups.memberships\n  method: post\n  operationId: groupsMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /groups.add_user\n  method: post\n  operationId: groupsAddUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /groups.remove_user\n  method: post\n  operationId: groupsRemoveUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /oauthClients.info\n  method: post\n  operationId: oauthClientsInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /oauthClients.list\n\
  \  method: post\n  operationId: oauthClientsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /oauthClients.create\n  method: post\n  operationId: oauthClientsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /oauthClients.update\n  method: post\n  operationId: oauthClientsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /oauthClients.rotate_secret\n  method: post\n  operationId: oauthClientsRotateSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /oauthClients.delete\n  method: post\n  operationId: oauthClientsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /oauthAuthentications.list\n  method:\
  \ post\n  operationId: oauthAuthenticationsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /oauthAuthentications.delete\n  method: post\n  operationId: oauthAuthenticationsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /revisions.info\n  method: post\n  operationId: revisionsInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /revisions.list\n  method: post\n  operationId: revisionsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience\n\n# --- truncated at 32 KB (41 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/agentic-access/outline-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/agentic-access/outline-agentic-access.yml
summary_line: 112 operations · 112 acting · 1 human-in-the-loop
tags:
- Knowledge Base
- Wiki
- Documents
- Collaboration
- Open-Source
- Team
---
