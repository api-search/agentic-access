---
acting_count: 96
action_class_counts:
  acting: 96
  connected: 25
api_specs:
- filename: utrecht-admin-api-openapi.yml
  format: yaml
  label: Utrecht University Admin API
  slug: utrecht-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-admin-api-openapi.yml
- filename: utrecht-browse-api-openapi.yml
  format: yaml
  label: Utrecht University Browse API
  slug: utrecht-browse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-browse-api-openapi.yml
- filename: utrecht-data-access-token-api-openapi.yml
  format: yaml
  label: Utrecht University Data Access Token API
  slug: utrecht-data-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-data-access-token-api-openapi.yml
- filename: utrecht-datarequest-api-openapi.yml
  format: yaml
  label: Utrecht University Datarequest API
  slug: utrecht-datarequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-datarequest-api-openapi.yml
- filename: utrecht-folder-api-openapi.yml
  format: yaml
  label: Utrecht University Folder API
  slug: utrecht-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-folder-api-openapi.yml
- filename: utrecht-groups-api-openapi.yml
  format: yaml
  label: Utrecht University Groups API
  slug: utrecht-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-groups-api-openapi.yml
- filename: utrecht-meta-api-openapi.yml
  format: yaml
  label: Utrecht University Meta API
  slug: utrecht-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-meta-api-openapi.yml
- filename: utrecht-meta-form-api-openapi.yml
  format: yaml
  label: Utrecht University Meta Form API
  slug: utrecht-meta-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-meta-form-api-openapi.yml
- filename: utrecht-notifications-api-openapi.yml
  format: yaml
  label: Utrecht University Notifications API
  slug: utrecht-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-notifications-api-openapi.yml
- filename: utrecht-provenance-api-openapi.yml
  format: yaml
  label: Utrecht University Provenance API
  slug: utrecht-provenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-provenance-api-openapi.yml
- filename: utrecht-publication-troubleshoot-api-openapi.yml
  format: yaml
  label: Utrecht University Publication Troubleshoot API
  slug: utrecht-publication-troubleshoot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-publication-troubleshoot-api-openapi.yml
- filename: utrecht-research-api-openapi.yml
  format: yaml
  label: Utrecht University Research API
  slug: utrecht-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-research-api-openapi.yml
- filename: utrecht-revisions-api-openapi.yml
  format: yaml
  label: Utrecht University Revisions API
  slug: utrecht-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-revisions-api-openapi.yml
- filename: utrecht-schema-api-openapi.yml
  format: yaml
  label: Utrecht University Schema API
  slug: utrecht-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-schema-api-openapi.yml
- filename: utrecht-schema-transformation-api-openapi.yml
  format: yaml
  label: Utrecht University Schema Transformation API
  slug: utrecht-schema-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-schema-transformation-api-openapi.yml
- filename: utrecht-settings-api-openapi.yml
  format: yaml
  label: Utrecht University Settings API
  slug: utrecht-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-settings-api-openapi.yml
- filename: utrecht-stats-api-openapi.yml
  format: yaml
  label: Utrecht University Stats API
  slug: utrecht-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-stats-api-openapi.yml
- filename: utrecht-vault-api-openapi.yml
  format: yaml
  label: Utrecht University Vault API
  slug: utrecht-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-vault-api-openapi.yml
- filename: utrecht-vault-archive-api-openapi.yml
  format: yaml
  label: Utrecht University Vault Archive API
  slug: utrecht-vault-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-vault-archive-api-openapi.yml
- filename: utrecht-vault-deaccession-api-openapi.yml
  format: yaml
  label: Utrecht University Vault Deaccession API
  slug: utrecht-vault-deaccession-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-vault-deaccession-api-openapi.yml
consequence_counts:
  physical: 1
  read: 25
  safety-critical: 4
  write: 91
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Utrecht Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /datarequest_attachment_upload_permission
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /datarequest_dta_upload_permission
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /datarequest_signed_dta_upload_permission
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /revoke_read_access_research_group
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /load_text_obj
operation_count: 121
overview: 'Utrecht University exposes 121 API operations that an AI agent could call, of which 96 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 91 write, 1 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Utrecht University
provider_slug: utrecht
slug: utrecht-agentic-access
source_filename: utrecht-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/utrecht-admin-api-openapi.yml, openapi/utrecht-browse-api-openapi.yml, openapi/utrecht-data-access-token-api-openapi.yml,\n  openapi/utrecht-datarequest-api-openapi.yml, openapi/utrecht-folder-api-openapi.yml, openapi/utrecht-groups-api-openapi.yml,\n  openapi/utrecht-meta-api-openapi.yml, openapi/utrecht-meta-form-api-openapi.yml, openapi/utrecht-notifications-api-openapi.yml,\n  openapi/utrecht-provenance-api-openapi.yml, openapi/utrecht-publication-troubleshoot-api-openapi.yml,\n  openapi/utrecht-research-api-openapi.yml, openapi/utrecht-revisions-api-openapi.yml, openapi/utrecht-schema-api-openapi.yml,\n  openapi/utrecht-schema-transformation-api-openapi.yml, openapi/utrecht-settings-api-openapi.yml,\n  openapi/utrecht-stats-api-openapi.yml, openapi/utrecht-vault-api-openapi.yml, openapi/utrecht-vault-archive-api-openapi.yml,\n  openapi/utrecht-vault-deaccession-api-openapi.yml\ndescription: Recommended x-agentic-access\
  \ execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 121\n  by_action_class:\n    acting: 96\n    connected: 25\n  by_consequence:\n    write: 91\n    physical: 1\n    read: 25\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /admin_has_access\n  method: post\n  operationId: postAdminHasAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browse_folder\n  method: post\n  operationId: postBrowseFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browse_collections\n  method: post\n  operationId: postBrowseCollections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  operationId: postSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /load_text_obj\n  method: post\n  operationId: postLoadTextObj\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token_generate\n  method: post\n  operationId: postTokenGenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token_load\n  method: post\n  operationId: postTokenLoad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token_delete\n  method: post\n  operationId: postTokenDelete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token_delete_expired\n  method: post\n  operationId: postTokenDeleteExpired\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_action_permitted\n  method: post\n  operationId: postDatarequestActionPermitted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /datarequest_roles_get\n  method: post\n  operationId: postDatarequestRolesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_schema_get\n  method: post\n  operationId: postDatarequestSchemaGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_resubmission_id_get\n  method: post\n  operationId: postDatarequestResubmissionIdGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /datarequest_browse\n  method: post\n  operationId: postDatarequestBrowse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_submit\n  method: post\n  operationId: postDatarequestSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_get\n  method: post\n  operationId: postDatarequestGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_attachment_upload_permission\n  method:\
  \ post\n  operationId: postDatarequestAttachmentUploadPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /datarequest_attachment_post_upload_actions\n  method: post\n  operationId: postDatarequestAttachmentPostUploadActions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_attachments_get\n  method: post\n  operationId: postDatarequestAttachmentsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /datarequest_attachments_submit\n  method: post\n  operationId: postDatarequestAttachmentsSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_preliminary_review_submit\n  method: post\n  operationId: postDatarequestPreliminaryReviewSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_preliminary_review_get\n  method: post\n  operationId: postDatarequestPreliminaryReviewGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_datamanager_review_submit\n  method: post\n  operationId: postDatarequestDatamanagerReviewSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_datamanager_review_get\n  method: post\n  operationId: postDatarequestDatamanagerReviewGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_dac_members_get\n  method: post\n  operationId: postDatarequestDacMembersGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_assignment_submit\n  method: post\n  operationId: postDatarequestAssignmentSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_assignment_get\n  method: post\n  operationId: postDatarequestAssignmentGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_review_submit\n  method: post\n  operationId: postDatarequestReviewSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_reviews_get\n  method: post\n  operationId: postDatarequestReviewsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_evaluation_submit\n  method: post\n  operationId: postDatarequestEvaluationSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_approval_conditions_get\n  method: post\n  operationId: postDatarequestApprovalConditionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_evaluation_get\n\
  \  method: post\n  operationId: postDatarequestEvaluationGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_feedback_get\n  method: post\n  operationId: postDatarequestFeedbackGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_preregistration_submit\n  method: post\n  operationId: postDatarequestPreregistrationSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_preregistration_get\n  method: post\n  operationId: postDatarequestPreregistrationGet\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_preregistration_confirm\n  method: post\n  operationId: postDatarequestPreregistrationConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_dta_upload_permission\n  method: post\n  operationId: postDatarequestDtaUploadPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /datarequest_dta_post_upload_actions\n  method: post\n  operationId: postDatarequestDtaPostUploadActions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_dta_path_get\n  method: post\n  operationId: postDatarequestDtaPathGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_signed_dta_upload_permission\n  method: post\n  operationId: postDatarequestSignedDtaUploadPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /datarequest_signed_dta_post_upload_actions\n  method: post\n  operationId: postDatarequestSignedDtaPostUploadActions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datarequest_signed_dta_path_get\n  method: post\n  operationId: postDatarequestSignedDtaPathGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datarequest_data_ready\n  method: post\n  operationId: postDatarequestDataReady\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folder_lock\n  method: post\n  operationId: postFolderLock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folder_unlock\n  method: post\n  operationId: postFolderUnlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folder_submit\n  method: post\n  operationId: postFolderSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folder_unsubmit\n  method: post\n  operationId: postFolderUnsubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folder_accept\n  method: post\n  operationId: postFolderAccept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folder_reject\n  method: post\n  operationId: postFolderReject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folder_get_locks\n  method: post\n  operationId: postFolderGetLocks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_get_user_role\n  method: post\n  operationId: postGroupGetUserRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group_data\n  method: post\n  operationId: postGroupData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group_process_csv\n\
  \  method: post\n  operationId: postGroupProcessCsv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_categories\n  method: post\n  operationId: postGroupCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group_subcategories\n  method: post\n  operationId: postGroupSubcategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group_search_users\n  method: post\n  operationId: postGroupSearchUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_exists\n  method: post\n  operationId: postGroupExists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_create\n  method: post\n  operationId: postGroupCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_update\n  method: post\n  operationId: postGroupUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_delete\n  method: post\n  operationId: postGroupDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_get_description\n  method: post\n  operationId: postGroupGetDescription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group_user_is_member\n  method: post\n  operationId: postGroupUserIsMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_user_add\n  method: post\n  operationId: postGroupUserAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_user_update_role\n  method: post\n  operationId: postGroupUserUpdateRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group_remove_user_from_group\n  method: post\n  operationId: postGroupRemoveUserFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meta_remove\n  method: post\n  operationId: postMetaRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meta_clone_file\n  method: post\n  operationId: postMetaCloneFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meta_form_load\n  method: post\n  operationId: postMetaFormLoad\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta_form_save\n  method: post\n  operationId: postMetaFormSave\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications_load\n  method: post\n  operationId: postNotificationsLoad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications_dismiss\n  method: post\n  operationId: postNotificationsDismiss\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications_dismiss_all\n  method: post\n  operationId: postNotificationsDismissAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provenance_log\n  method: post\n  operationId: postProvenanceLog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch_troubleshoot_published_data_packages\n  method: post\n\
  \  operationId: postBatchTroubleshootPublishedDataPackages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_folder_add\n  method: post\n  operationId: postResearchFolderAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_folder_copy\n  method: post\n  operationId: postResearchFolderCopy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /research_folder_move\n  method: post\n  operationId: postResearchFolderMove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_folder_rename\n  method: post\n  operationId: postResearchFolderRename\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_folder_delete\n  method: post\n  operationId: postResearchFolderDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_list_temporary_files\n  method: post\n  operationId: postResearchListTemporaryFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /research_file_copy\n  method: post\n  operationId: postResearchFileCopy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_file_rename\n  method: post\n  operationId: postResearchFileRename\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_file_move\n  method: post\n  operationId: postResearchFileMove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_file_delete\n  method: post\n  operationId: postResearchFileDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_system_metadata\n  method: post\n  operationId: postResearchSystemMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_collection_details\n  method: post\n  operationId: postResearchCollectionDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research_manifest\n  method: post\n  operationId: postResearchManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /revisions_search_on_filename\n  method: post\n  operationId:\
  \ postRevisionsSearchOnFilename\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /revisions_list\n  method: post\n  operationId: postRevisionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /revisions_restore\n  method: post\n  operationId: postRevisionsRestore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schema_get_schemas\n  method: post\n  operationId: postSchemaGetSchemas\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transform_metadata\n  method: post\n  operationId: postTransformMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings_load\n  method: post\n  operationId: postSettingsLoad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings_save\n  method: post\n  operationId:\
  \ postSettingsSave\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resource_browse_group_data\n  method: post\n  operationId: postResourceBrowseGroupData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource_full_year_differentiated_group_storage\n  method: post\n  operationId: postResourceFullYearDifferentiatedGroupStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (40 KB total) ---\n\
  # Full source: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/agentic-access/utrecht-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/agentic-access/utrecht-agentic-access.yml
summary_line: 121 operations · 96 acting · 4 human-in-the-loop
tags:
- Education
- Higher Education
- University
- Netherlands
- Europe
- Research Data
- Research Data Management
- Institutional Repository
- Identity Federation
- OAI-PMH
- Open Access
- Open Science
- Library
- Open Source
---
