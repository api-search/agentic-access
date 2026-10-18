---
acting_count: 94
action_class_counts:
  acting: 94
  connected: 55
api_specs:
- filename: popp-agents-api-openapi.yml
  format: yaml
  label: Popp Agents API
  slug: popp-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-agents-api-openapi.yml
- filename: popp-analysis-api-openapi.yml
  format: yaml
  label: Popp Analysis API
  slug: popp-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-analysis-api-openapi.yml
- filename: popp-ats-api-openapi.yml
  format: yaml
  label: Popp ATS API
  slug: popp-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-ats-api-openapi.yml
- filename: popp-campaigns-api-openapi.yml
  format: yaml
  label: Popp Campaigns API
  slug: popp-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-campaigns-api-openapi.yml
- filename: popp-candidate-lists-api-openapi.yml
  format: yaml
  label: Popp Candidate Lists API
  slug: popp-candidate-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-candidate-lists-api-openapi.yml
- filename: popp-candidates-api-openapi.yml
  format: yaml
  label: Popp Candidates API
  slug: popp-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-candidates-api-openapi.yml
- filename: popp-conversations-api-openapi.yml
  format: yaml
  label: Popp Conversations API
  slug: popp-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-conversations-api-openapi.yml
- filename: popp-custom-fields-beta-api-openapi.yml
  format: yaml
  label: Popp Custom Fields (Beta) API
  slug: popp-custom-fields-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-custom-fields-beta-api-openapi.yml
- filename: popp-document-credentials-api-openapi.yml
  format: yaml
  label: Popp Document Credentials API
  slug: popp-document-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-document-credentials-api-openapi.yml
- filename: popp-documents-api-openapi.yml
  format: yaml
  label: Popp Documents API
  slug: popp-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-documents-api-openapi.yml
- filename: popp-organization-configuration-api-openapi.yml
  format: yaml
  label: Popp Organization Configuration API
  slug: popp-organization-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-organization-configuration-api-openapi.yml
- filename: popp-organizations-api-openapi.yml
  format: yaml
  label: Popp Organizations API
  slug: popp-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-organizations-api-openapi.yml
- filename: popp-scheduling-api-openapi.yml
  format: yaml
  label: Popp Scheduling API
  slug: popp-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-scheduling-api-openapi.yml
- filename: popp-tags-api-openapi.yml
  format: yaml
  label: Popp Tags API
  slug: popp-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-tags-api-openapi.yml
- filename: popp-templates-api-openapi.yml
  format: yaml
  label: Popp Templates API
  slug: popp-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-templates-api-openapi.yml
- filename: popp-users-api-openapi.yml
  format: yaml
  label: Popp Users API
  slug: popp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-users-api-openapi.yml
- filename: popp-webhooks-api-openapi.yml
  format: yaml
  label: Popp Webhooks API
  slug: popp-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-webhooks-api-openapi.yml
- filename: popp-workflows-api-openapi.yml
  format: yaml
  label: Popp Workflows API
  slug: popp-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-workflows-api-openapi.yml
consequence_counts:
  physical: 2
  read: 55
  safety-critical: 1
  write: 91
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Popp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/campaigns/{campaignId}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/conversations/resend-booking-url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/conversations/{conversationId}/messages
operation_count: 149
overview: 'Popp exposes 149 API operations that an AI agent could call, of which 94 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 55 read, 91 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Popp
provider_slug: popp
slug: popp-agentic-access
source_filename: popp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/popp-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 149\n  by_action_class:\n    connected: 55\n    acting: 94\n  by_consequence:\n    read: 55\n    write: 91\n    safety-critical: 1\n    physical: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/agents\n  method: get\n  operationId: list-agents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyses\n  method: post\n  operationId: create-analysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analyses\n  method: get\n  operationId: list-analyses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyses/generate-requirements\n  method: post\n  operationId: generate-requirements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analyses/{id}\n  method: get\n  operationId: get-analysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyses/{id}\n  method: put\n  operationId: update-analysis\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analyses/{id}/archive\n  method: post\n  operationId: archive-analysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analyses/{id}/update-requirements-and-reanalyse\n  method: post\n  operationId: update-requirements-and-reanalyse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/analysis/candidates\n  method: post\n  operationId: create-analysis-candidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ats/jobs\n  method: get\n  operationId: list-ats-jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ats/jobs/{atsJobId}/stages\n  method: get\n  operationId: list-ats-job-stages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ats/rejection-reasons\n  method: get\n  operationId: list-ats-rejection-reasons\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/availability/parse\n  method: post\n  operationId: parse-availability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings\n  method: get\n  operationId: list-bookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}\n  method: patch\n  operationId: update-booking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/bookings/{bookingId}\n  method: get\n  operationId: get-booking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}/cancel\n  method: post\n  operationId: cancel-booking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns\n  method: post\n  operationId: create-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns\n  method: get\n  operationId:\
  \ list-campaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{campaignId}\n  method: get\n  operationId: get-campaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{campaignId}\n  method: put\n  operationId: update-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns/{campaignId}/stop\n  method: post\n  operationId: stop-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/candidate-profiles/by-external-id/{externalId}\n  method: get\n  operationId: get-candidate-profile-by-external-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates\n  method: post\n  operationId: create-candidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/by-email/{email}\n  method: delete\n  operationId: delete-candidate-by-email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/by-external-id/{externalId}\n  method: patch\n  operationId: update-candidate-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/by-external-id/{externalId}\n  method: get\n  operationId: get-candidate-by-external-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates/by-external-id/{externalId}\n  method: delete\n  operationId: delete-candidate-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/by-external-id/{externalId}/document\n  method: delete\n  operationId: remove-candidate-document-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/by-external-id/{externalId}/notes\n  method: get\n  operationId: list-candidate-notes-by-external-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates/by-external-id/{externalId}/notes\n  method: post\n  operationId: create-candidate-note-by-external-id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/by-external-id/{externalId}/reparse\n  method: post\n  operationId: reparse-candidate-cv-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/by-phone-number/{phoneNumber}\n  method: delete\n  operationId: delete-candidate-by-phone-number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/lists\n  method: get\n  operationId: list-candidate-lists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates/lists\n  method: post\n  operationId: create-candidate-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/lists/by-external-id/{externalId}\n  method: get\n  operationId: get-candidate-list-by-external-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates/lists/by-external-id/{externalId}\n  method:\
  \ patch\n  operationId: update-candidate-list-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/lists/by-external-id/{externalId}\n  method: delete\n  operationId: delete-candidate-list-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/lists/by-external-id/{externalId}/candidates\n  method: post\n  operationId: add-candidates-to-list-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/lists/by-external-id/{externalId}/candidates\n  method: delete\n  operationId: remove-candidates-from-list-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/lists/{id}\n  method: get\n  operationId: get-candidate-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates/lists/{id}\n  method: patch\n  operationId: update-candidate-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/lists/{id}\n  method: delete\n  operationId: delete-candidate-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/lists/{id}/candidates\n  method: post\n  operationId: add-candidates-to-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/lists/{id}/candidates\n  method: delete\n  operationId:\
  \ remove-candidates-from-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/tags\n  method: get\n  operationId: list-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates/tags/{id}\n  method: delete\n  operationId: delete-tag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/{id}\n  method: patch\n  operationId: update-candidate\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/{id}\n  method: get\n  operationId: get-candidate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates/{id}\n  method: delete\n  operationId: delete-candidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/{id}/document\n  method: delete\n  operationId: remove-candidate-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/{id}/notes\n  method: get\n  operationId: list-candidate-notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates/{id}/notes\n  method: post\n  operationId: create-candidate-note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/{id}/notes/{noteId}\n  method: patch\n  operationId: update-candidate-note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/{id}/notes/{noteId}\n  method: delete\n  operationId: delete-candidate-note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/{id}/reparse\n  method: post\n  operationId: reparse-candidate-cv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config\n  method: get\n  operationId: get-organization-config\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config\n  method: post\n  operationId: create-organization-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config\n  method: patch\n  operationId: update-organization-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/by-external-organization-id/{externalOrganizationId}\n  method: get\n  operationId: get-organization-config-by-external-id\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/by-external-organization-id/{externalOrganizationId}\n  method: patch\n  operationId: update-organization-config-by-external-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conversations\n  method: post\n  operationId: create-conversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conversations\n  method: get\n  operationId: list-conversations\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conversations/bulk\n  method: post\n  operationId: bulk-create-conversations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conversations/resend-booking-url\n  method: post\n  operationId: resend-booking-url\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conversations/{conversationId}\n  method: get\n  operationId: get-conversation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conversations/{conversationId}/documents\n  method: get\n  operationId: list-conversation-documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conversations/{conversationId}/hand-to-agent\n  method: post\n  operationId: hand-conversation-to-agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conversations/{conversationId}/messages\n  method: get\n  operationId: list-conversation-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conversations/{conversationId}/messages\n  method: post\n  operationId: send-conversation-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conversations/{conversationId}/takeover\n  method: post\n  operationId: takeover-conversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/custom-fields\n  method: post\n  operationId: create-custom-field\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/custom-fields\n  method: get\n  operationId: list-custom-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/custom-fields/{id}\n  method: get\n  operationId: get-custom-field\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/custom-fields/{id}\n  method: patch\n  operationId: update-custom-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/custom-fields/{id}\n  method: delete\n  operationId: delete-custom-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document-credentials\n  method: post\n  operationId: create-document-credential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document-credentials\n  method: get\n  operationId: list-document-credentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/document-credentials/{id}\n  method: patch\n  operationId: update-document-credential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document-credentials/{id}\n  method: delete\n  operationId: delete-document-credential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document-types\n  method: get\n  operationId: list-document-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/document-types\n\
  \  method: post\n  operationId: create-document-type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document-types/{documentTypeId}\n  method: get\n  operationId: get-document-type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/document-types/{documentTypeId}\n  method: patch\n  operationId: update-document-type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document-types/{documentTypeId}\n  method:\
  \ delete\n  operationId: delete-document-type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document-types/{documentTypeId}/archive\n  method: post\n  operationId: archive-document-type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/process\n  method: post\n  operationId: process-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{documentId}\n  method: get\n  operationId: get-document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{documentId}/media\n  method: get\n  operationId: get-document-media\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{documentId}/media/download\n  method: get\n  operationId: download-media\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/generate-preferred-answer-requirements\n  method: post\n  operationId: generate-preferred-answer-requirements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generate-questions\n  method: post\n  operationId: generate-questions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invite-calendar-contact\n  method: post\n  operationId: invite-calendar-contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meeting-templates\n  method: get\n  operationId: list-meeting-templates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meeting-templates\n  method: post\n  operationId: create-meeting-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meeting-templates/{templateId}\n  method: get\n  operationId: get-meeting-template\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meeting-templates/{templateId}\n  method: put\n  operationId: update-meeting-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meeting-templates/{templateId}\n  method: delete\n  operationId: delete-meeting-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations\n  method: get\n  operationId: list-organizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{id}\n  method: patch\n  operationId: update-organization-details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{id}\n  method: get\n  operationId: get-organization-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{id}/users\n  method: get\n  operationId: list-organization-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scheduling/conversations\n  method: post\n  operationId: create-scheduling-conversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (45 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/agentic-access/popp-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/agentic-access/popp-agentic-access.yml
summary_line: 149 operations · 94 acting · 1 human-in-the-loop
tags:
- Company
- Recruiting
- Staffing
- Hiring
- Conversational AI
- Automation
- Scheduling
- Workflows
- Webhook
- MCP
- Agents
---
