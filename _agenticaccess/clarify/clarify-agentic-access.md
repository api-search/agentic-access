---
acting_count: 56
action_class_counts:
  acting: 56
  connected: 29
api_specs:
- filename: clarify-activities-api-openapi.yml
  format: yaml
  label: Clarify Activities API
  slug: clarify-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-activities-api-openapi.yml
- filename: clarify-campaigns-api-openapi.yml
  format: yaml
  label: Clarify Campaigns API
  slug: clarify-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-campaigns-api-openapi.yml
- filename: clarify-comments-api-openapi.yml
  format: yaml
  label: Clarify Comments API
  slug: clarify-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-comments-api-openapi.yml
- filename: clarify-invitations-api-openapi.yml
  format: yaml
  label: Clarify Invitations API
  slug: clarify-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-invitations-api-openapi.yml
- filename: clarify-layouts-api-openapi.yml
  format: yaml
  label: Clarify Layouts API
  slug: clarify-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-layouts-api-openapi.yml
- filename: clarify-listrows-api-openapi.yml
  format: yaml
  label: Clarify List Rows API
  slug: clarify-listrows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-listrows-api-openapi.yml
- filename: clarify-lists-api-openapi.yml
  format: yaml
  label: Clarify Lists API
  slug: clarify-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-lists-api-openapi.yml
- filename: clarify-meetingrecordings-api-openapi.yml
  format: yaml
  label: Clarify Meeting Recordings API
  slug: clarify-meetingrecordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-meetingrecordings-api-openapi.yml
- filename: clarify-objectaccess-api-openapi.yml
  format: yaml
  label: Clarify Object Access API
  slug: clarify-objectaccess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-objectaccess-api-openapi.yml
- filename: clarify-recordaccess-api-openapi.yml
  format: yaml
  label: Clarify Record Access API
  slug: clarify-recordaccess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-recordaccess-api-openapi.yml
- filename: clarify-recordattachments-api-openapi.yml
  format: yaml
  label: Clarify Record Attachments API
  slug: clarify-recordattachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-recordattachments-api-openapi.yml
- filename: clarify-recordrelationships-api-openapi.yml
  format: yaml
  label: Clarify Record Relationships API
  slug: clarify-recordrelationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-recordrelationships-api-openapi.yml
- filename: clarify-records-api-openapi.yml
  format: yaml
  label: Clarify Records API
  slug: clarify-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-records-api-openapi.yml
- filename: clarify-resources-api-openapi.yml
  format: yaml
  label: Clarify Resources API
  slug: clarify-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-resources-api-openapi.yml
- filename: clarify-schemas-api-openapi.yml
  format: yaml
  label: Clarify Schemas API
  slug: clarify-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-schemas-api-openapi.yml
- filename: clarify-users-api-openapi.yml
  format: yaml
  label: Clarify Users API
  slug: clarify-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-users-api-openapi.yml
- filename: clarify-workflows-api-openapi.yml
  format: yaml
  label: Clarify Workflows API
  slug: clarify-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-workflows-api-openapi.yml
- filename: clarify-workspacesettings-api-openapi.yml
  format: yaml
  label: Clarify Workspace Settings API
  slug: clarify-workspacesettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-workspacesettings-api-openapi.yml
- filename: clarify-api-keys-api-openapi.yml
  format: yaml
  label: Clarify API Keys API
  slug: clarify-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/openapi/clarify-api-keys-api-openapi.yml
consequence_counts:
  physical: 6
  read: 29
  safety-critical: 6
  write: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Clarify Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /workspaces/{workspace}/invitations/{invitationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspaces/{workspace}/layouts/{id}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /workspaces/{workspace}/meetings/{meetingId}/recording
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /workspaces/{workspace}/objects/{object}/access/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /workspaces/{workspace}/objects/{object}/records/{id}/access/{grantId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /workspaces/{workspace}/settings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspace}/invitations/{invitationId}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /workspaces/{workspace}/objects/{object}/records/{id}/relationships/{relationship}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /workspaces/{workspace}/objects/{object}/records/{id}/relationships/{relationship}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /workspaces/{workspace}/schemas/{entity}/fields-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspace}/schemas/{entity}/relationships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /workspaces/{workspace}/schemas/{entity}/relationships/{fieldName}
operation_count: 85
overview: 'Clarify exposes 85 API operations that an AI agent could call, of which 56 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 44 write, 6 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clarify
provider_slug: clarify
slug: clarify-agentic-access
source_filename: clarify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: generated\nsource: openapi/clarify-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 85\n  by_action_class:\n    connected: 29\n    acting: 56\n  by_consequence:\n    read: 29\n    write: 44\n    safety-critical: 6\n    physical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /workspaces/{workspace}/objects/{object}/records/{record}/activities\n  method: get\n  operationId: getActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/api-keys\n  method: get\n  operationId: getApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/api-keys/{id}\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/campaigns/{campaignId}/recipients\n  method: get\n  operationId: getRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/comments\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/comments/{id}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/comments/{id}\n  method: patch\n  operationId: updateComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /workspaces/{workspace}/comments/{id}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/layouts/{id}\n  method: get\n  operationId: getLayoutById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/layouts/{id}\n  method: patch\n  operationId: updateLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /workspaces/{workspace}/layouts/{id}/reset\n  method: post\n  operationId: resetLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/lists\n  method: get\n  operationId: getLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/lists\n  method: post\n  operationId: createList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/lists/{list}\n  method: get\n  operationId: getList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/lists/{list}\n  method: patch\n  operationId: updateList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/lists/{list}\n  method: delete\n  operationId: deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/lists/{list}/publish\n  method: post\n  operationId: publishList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/lists/{list}/unpublish\n  method: post\n  operationId: unpublishList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/lists/{list}/rows/csv\n  method: post\n  operationId: getListRowsCsv\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/lists\n  method: get\n  operationId: getWorkspaceLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/meetings/{meetingId}/recording\n  method: post\n  operationId: enableRecording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/meetings/{meetingId}/recording\n  method: delete\n  operationId: disableRecording\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /workspaces/{workspace}/meetings/{meetingId}/recordings/{id}/artifacts\n  method: post\n  operationId: getRecordingArtifacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/meetings/{meetingId}/recordings/transcript\n  method: post\n  operationId: uploadRecordingTranscript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/meetings/{meetingId}/recordings/media\n  method: post\n  operationId: initMediaUpload\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/meetings/{meetingId}/recordings/media/{recordingId}\n  method: post\n  operationId: confirmMediaUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/meetings/{meetingId}/transcript\n  method: post\n  operationId: uploadTranscript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/access\n  method: get\n  operationId: getObjectAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/access\n  method: post\n  operationId: giveObjectAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/access/{id}\n  method: delete\n  operationId: revokeObjectAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n \
  \     proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/access\n  method: get\n  operationId: getGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/access\n  method: post\n  operationId: createGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/access/bulk\n  method: post\n  operationId: createGrantsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/access/{grantId}\n  method: patch\n  operationId: updateGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/access/{grantId}\n  method: delete\n  operationId: revokeGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /workspaces/{workspace}/objects/{object}/records/{id}\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/records/{id}\n  method: patch\n  operationId: updateRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}\n  method: delete\n  operationId: deleteRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /workspaces/{workspace}/objects/{object}/records\n  method: post\n  operationId: createRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records\n  method: patch\n  operationId: updateRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records\n  method: delete\n  operationId: deleteRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/bulk\n  method: post\n  operationId: createBulkRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/relationships/{relationship}\n  method: get\n  operationId: getRecordRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/relationships/{relationship}\n  method: patch\n  operationId: updateRecordRelationship\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/relationships/{relationship}\n  method: delete\n  operationId: deleteRecordRelationship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/attachments\n  method: get\n  operationId: listRecordAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/attachments\n  method: post\n  operationId: addRecordAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/attachments\n  method: put\n  operationId: getSignedUrlForRecordAttachmentUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/attachments/{attachmentId}\n  method: get\n\
  \  operationId: getRecordAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/records/{id}/attachments/{attachmentId}\n  method: delete\n  operationId: deleteRecordAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/records/{record}/merges\n  method: post\n  operationId: mergeRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /workspaces/{workspace}/objects/{object}/resources/{id}\n  method: get\n  operationId: getResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/resources\n  method: get\n  operationId: getResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/resources\n  method: post\n  operationId: createResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/objects/{object}/lists/{list}/resources\n  method: get\n  operationId: getListResources\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/objects/{object}/deleted-resources\n  method: get\n  operationId: getDeletedResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/schemas\n  method: get\n  operationId: getSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/schemas\n  method: patch\n  operationId: patchEnumFieldValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /workspaces/{workspace}/schemas/objects\n  method: post\n  operationId: createCustomObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/schemas/objects/{object}\n  method: put\n  operationId: updateEntitySchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/schemas/objects/{object}\n  method: delete\n  operationId: deleteCustomObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/schemas/{entity}/fields-order\n  method: patch\n  operationId: updateSchemaPropertyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/schemas/{entity}/fields-visibility\n  method: patch\n  operationId: updateSchemaPropertyVisibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /workspaces/{workspace}/schemas/{entity}/properties\n  method: post\n  operationId: createSchemaProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/schemas/{entity}/relationships\n  method: post\n  operationId: createSchemaRelationshipProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/schemas/{entity}/relationships/{fieldName}\n  method: delete\n  operationId: deleteSchemaRelationshipProperty\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/schemas/{entity}/activities\n  method: get\n  operationId: getSchemaActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/users/{userId}\n  method: delete\n  operationId: removeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/users/{userId}/role\n  method: patch\n  operationId: updateUserRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/settings\n  method: get\n  operationId: readAllWorkspaceSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/settings\n  method: post\n  operationId: writeWorkspaceSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/settings\n  method: delete\n  operationId: deleteWorkspaceSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /workspaces/{workspace}/settings/{key}\n  method: get\n  operationId: readWorkspaceSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/workflows/{id}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/workflows/{id}\n  method: patch\n  operationId: updateWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/workflows/{id}\n  method: delete\n  operationId: deleteWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/workflows\n  method: get\n  operationId: getWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/workflows\n  method: post\n  operationId: createWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/invitations\n  method: get\n  operationId: getInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace}/invitations\n  method: post\n  operationId: createInvitation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace}/invitations/{invitationId}\n  method: delete\n  operationId: revokeInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /workspaces/{workspace}/invitations/{invitationId}/resend\n  method: post\n  operationId: resendInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarify/refs/heads/main/agentic-access/clarify-agentic-access.yml
summary_line: 85 operations · 56 acting · 6 human-in-the-loop
tags:
- Company
- CRM
- Artificial Intelligence
- Automation
- Sales
---
