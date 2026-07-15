---
acting_count: 627
action_class_counts:
  acting: 627
  connected: 498
api_specs:
- filename: gitlab-ci-openapi.yml
  format: yaml
  label: GitLab REST API v4 (CI/CD endpoints)
  slug: rest-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab-ci/refs/heads/main/openapi/gitlab-ci-openapi.yml
consequence_counts:
  physical: 21
  read: 498
  safety-critical: 22
  write: 584
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 22
kind: agentic-access
layout: agentic-access
method: generated
name: Gitlab Ci Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v4/groups/{id}/integrations/{slug}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/groups/{id}/members/{user_id}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v4/groups/{id}/members/{user_id}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/groups/{id}/runners/reset_registration_token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v4/personal_access_tokens/self
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v4/personal_access_tokens/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v4/projects/{id}/cluster_agents/{agent_id}/tokens/{token_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v4/projects/{id}/environments/review_apps
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/projects/{id}/environments/stop_stale
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/projects/{id}/environments/{environment_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v4/projects/{id}/error_tracking/settings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v4/projects/{id}/integrations/{slug}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/projects/{id}/issues/{issue_iid}/reset_spent_time
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/projects/{id}/issues/{issue_iid}/reset_time_estimate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v4/projects/{id}/merge_requests/{merge_request_iid}/reset_approvals
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/projects/{id}/merge_requests/{merge_request_iid}/reset_spent_time
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/projects/{id}/merge_requests/{merge_request_iid}/reset_time_estimate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/projects/{id}/runners/reset_registration_token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v4/projects/{id}/services/{slug}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/runners/reset_authentication_token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/runners/reset_registration_token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/runners/{id}/reset_authentication_token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v4/deploy_keys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v4/groups/{id}/deploy_tokens
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v4/groups/{id}/deploy_tokens/{token_id}
operation_count: 1125
overview: 'GitLab CI/CD exposes 1125 API operations that an AI agent could call, of which 627 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 498 read, 584 write, 21 physical, and 22 safety-critical.


  22 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GitLab CI/CD
provider_slug: gitlab-ci
slug: gitlab-ci-agentic-access
source_filename: gitlab-ci-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gitlab-ci-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1125\n  by_action_class:\n    connected: 498\n    acting: 627\n  by_consequence:\n    read: 498\n    write: 584\n    physical: 21\n    safety-critical: 22\n  human_in_the_loop_required: 22\noperations:\n- path: /api/v4/groups/{id}/access_requests\n  method: get\n  operationId: getApiV4GroupsIdAccessRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/access_requests\n  method: post\n  operationId: postApiV4GroupsIdAccessRequests\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/access_requests/{user_id}/approve\n  method: put\n  operationId: putApiV4GroupsIdAccessRequestsUserIdApprove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/access_requests/{user_id}\n  method: delete\n  operationId: deleteApiV4GroupsIdAccessRequestsUserId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /api/v4/groups/{id}/epics/{epic_iid}/award_emoji\n  method: get\n  operationId: getApiV4GroupsIdEpicsEpicIidAwardEmoji\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/epics/{epic_iid}/award_emoji\n  method: post\n  operationId: postApiV4GroupsIdEpicsEpicIidAwardEmoji\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/epics/{epic_iid}/award_emoji/{award_id}\n  method: get\n  operationId: getApiV4GroupsIdEpicsEpicIidAwardEmojiAwardId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v4/groups/{id}/epics/{epic_iid}/award_emoji/{award_id}\n  method: delete\n  operationId: deleteApiV4GroupsIdEpicsEpicIidAwardEmojiAwardId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/epics/{epic_iid}/notes/{note_id}/award_emoji\n  method: get\n  operationId: getApiV4GroupsIdEpicsEpicIidNotesNoteIdAwardEmoji\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/epics/{epic_iid}/notes/{note_id}/award_emoji\n  method: post\n  operationId: postApiV4GroupsIdEpicsEpicIidNotesNoteIdAwardEmoji\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/epics/{epic_iid}/notes/{note_id}/award_emoji/{award_id}\n  method: get\n  operationId: getApiV4GroupsIdEpicsEpicIidNotesNoteIdAwardEmojiAwardId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/epics/{epic_iid}/notes/{note_id}/award_emoji/{award_id}\n  method: delete\n  operationId: deleteApiV4GroupsIdEpicsEpicIidNotesNoteIdAwardEmojiAwardId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/badges\n  method: get\n  operationId:\
  \ getApiV4GroupsIdBadges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/badges\n  method: post\n  operationId: postApiV4GroupsIdBadges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/badges/render\n  method: get\n  operationId: getApiV4GroupsIdBadgesRender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/badges/{badge_id}\n  method: get\n  operationId: getApiV4GroupsIdBadgesBadgeId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/badges/{badge_id}\n  method: put\n  operationId: putApiV4GroupsIdBadgesBadgeId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/badges/{badge_id}\n  method: delete\n  operationId: deleteApiV4GroupsIdBadgesBadgeId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/custom_attributes\n  method: get\n  operationId: getApiV4GroupsIdCustomAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/custom_attributes/{key}\n  method: get\n  operationId: getApiV4GroupsIdCustomAttributesKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/custom_attributes/{key}\n  method: put\n  operationId: putApiV4GroupsIdCustomAttributesKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/custom_attributes/{key}\n  method: delete\n  operationId: deleteApiV4GroupsIdCustomAttributesKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups\n  method: get\n  operationId: getApiV4Groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups\n  method: post\n  operationId: postApiV4Groups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}\n  method: put\n  operationId: putApiV4GroupsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}\n  method: get\n  operationId: getApiV4GroupsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}\n  method: delete\n  operationId: deleteApiV4GroupsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/archive\n  method: post\n  operationId: postApiV4GroupsIdArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v4/groups/{id}/unarchive\n  method: post\n  operationId: postApiV4GroupsIdUnarchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/restore\n  method: post\n  operationId: postApiV4GroupsIdRestore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/groups/shared\n  method: get\n  operationId: getApiV4GroupsIdGroupsShared\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v4/groups/{id}/invited_groups\n  method: get\n  operationId: getApiV4GroupsIdInvitedGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/projects\n  method: get\n  operationId: getApiV4GroupsIdProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/projects/shared\n  method: get\n  operationId: getApiV4GroupsIdProjectsShared\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/subgroups\n  method: get\n  operationId: getApiV4GroupsIdSubgroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v4/groups/{id}/descendant_groups\n  method: get\n  operationId: getApiV4GroupsIdDescendantGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/projects/{project_id}\n  method: post\n  operationId: postApiV4GroupsIdProjectsProjectId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/transfer_locations\n  method: get\n  operationId: getApiV4GroupsIdTransferLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/transfer\n  method: post\n  operationId: postApiV4GroupsIdTransfer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/transfer_to_organization\n  method: post\n  operationId: postApiV4GroupsIdTransferToOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/share\n  method: post\n  operationId: postApiV4GroupsIdShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/share/{group_id}\n  method: delete\n  operationId: deleteApiV4GroupsIdShareGroupId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/ldap_sync\n  method: post\n  operationId: postApiV4GroupsIdLdapSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/audit_events\n  method: get\n  operationId: getApiV4GroupsIdAuditEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/audit_events/{audit_event_id}\n  method: get\n  operationId: getApiV4GroupsIdAuditEventsAuditEventId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/saml_users\n  method: get\n  operationId: getApiV4GroupsIdSamlUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/provisioned_users\n  method: get\n  operationId: getApiV4GroupsIdProvisionedUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/ssh_certificates\n  method: get\n  operationId: getApiV4GroupsIdSshCertificates\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/ssh_certificates\n  method: post\n  operationId: postApiV4GroupsIdSshCertificates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/ssh_certificates/{ssh_certificates_id}\n  method: delete\n  operationId: deleteApiV4GroupsIdSshCertificatesSshCertificatesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/runners\n\
  \  method: get\n  operationId: getApiV4GroupsIdRunners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/runners/reset_registration_token\n  method: post\n  operationId: postApiV4GroupsIdRunnersResetRegistrationToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v4/groups/{id}/-/packages/debian/dists/*distribution/Release.gpg\n  method: get\n  operationId: getApiV4GroupsIdPackagesDebianDists*distributionReleaseGpg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/packages/debian/dists/*distribution/Release\n\
  \  method: get\n  operationId: getApiV4GroupsIdPackagesDebianDists*distributionRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/packages/debian/dists/*distribution/InRelease\n  method: get\n  operationId: getApiV4GroupsIdPackagesDebianDists*distributionInrelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/packages/debian/dists/*distribution/{component}/debian-installer/binary-{architecture}/Packages\n  method: get\n  operationId: getApiV4GroupsIdPackagesDebianDists*distributionComponentDebianInstallerBinaryArchitecturePackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/packages/debian/dists/*distribution/{component}/debian-installer/binary-{architecture}/by-hash/SHA256/{file_sha256}\n\
  \  method: get\n  operationId: getApiV4GroupsIdPackagesDebianDists*distributionComponentDebianInstallerBinaryArchitectureByHashSha256FileSha256\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/packages/debian/dists/*distribution/{component}/source/Sources\n  method: get\n  operationId: getApiV4GroupsIdPackagesDebianDists*distributionComponentSourceSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/packages/debian/dists/*distribution/{component}/source/by-hash/SHA256/{file_sha256}\n  method: get\n  operationId: getApiV4GroupsIdPackagesDebianDists*distributionComponentSourceByHashSha256FileSha256\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v4/groups/{id}/-/packages/debian/dists/*distribution/{component}/binary-{architecture}/Packages\n  method: get\n  operationId: getApiV4GroupsIdPackagesDebianDists*distributionComponentBinaryArchitecturePackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/packages/debian/dists/*distribution/{component}/binary-{architecture}/by-hash/SHA256/{file_sha256}\n  method: get\n  operationId: getApiV4GroupsIdPackagesDebianDists*distributionComponentBinaryArchitectureByHashSha256FileSha256\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/packages/debian/pool/{distribution}/{project_id}/{letter}/{package_name}/{package_version}/{file_name}\n  method: get\n  operationId: getApiV4GroupsIdPackagesDebianPoolDistributionProjectIdLetterPackageNamePackageVersionFileName\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/dependency_proxy/cache\n  method: delete\n  operationId: deleteApiV4GroupsIdDependencyProxyCache\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/deploy_tokens\n  method: get\n  operationId: getApiV4GroupsIdDeployTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/deploy_tokens\n  method: post\n  operationId: postApiV4GroupsIdDeployTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/deploy_tokens/{token_id}\n  method: get\n  operationId: getApiV4GroupsIdDeployTokensTokenId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/deploy_tokens/{token_id}\n  method: delete\n  operationId: deleteApiV4GroupsIdDeployTokensTokenId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/avatar\n \
  \ method: get\n  operationId: getApiV4GroupsIdAvatar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/clusters\n  method: get\n  operationId: getApiV4GroupsIdClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/clusters/{cluster_id}\n  method: get\n  operationId: getApiV4GroupsIdClustersClusterId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/clusters/{cluster_id}\n  method: put\n  operationId: putApiV4GroupsIdClustersClusterId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/clusters/{cluster_id}\n  method: delete\n  operationId: deleteApiV4GroupsIdClustersClusterId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/clusters/user\n  method: post\n  operationId: postApiV4GroupsIdClustersUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/registry/repositories\n  method: get\n  operationId: getApiV4GroupsIdRegistryRepositories\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/debian_distributions\n  method: post\n  operationId: postApiV4GroupsIdDebianDistributions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/-/debian_distributions\n  method: get\n  operationId: getApiV4GroupsIdDebianDistributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/debian_distributions/{codename}\n  method: get\n  operationId: getApiV4GroupsIdDebianDistributionsCodename\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/-/debian_distributions/{codename}\n  method: put\n  operationId: putApiV4GroupsIdDebianDistributionsCodename\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/-/debian_distributions/{codename}\n  method: delete\n  operationId: deleteApiV4GroupsIdDebianDistributionsCodename\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/-/debian_distributions/{codename}/key.asc\n  method: get\n  operationId:\
  \ getApiV4GroupsIdDebianDistributionsCodenameKeyAsc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/export/download\n  method: get\n  operationId: getApiV4GroupsIdExportDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/export\n  method: post\n  operationId: postApiV4GroupsIdExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/export_relations\n  method: post\n  operationId: postApiV4GroupsIdExportRelations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/export_relations/download\n  method: get\n  operationId: getApiV4GroupsIdExportRelationsDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/export_relations/status\n  method: get\n  operationId: getApiV4GroupsIdExportRelationsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/import/authorize\n  method: post\n  operationId: postApiV4GroupsImportAuthorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/import\n  method: post\n  operationId: postApiV4GroupsImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/packages\n  method: get\n  operationId: getApiV4GroupsIdPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/placeholder_reassignments\n  method: get\n  operationId: getApiV4GroupsIdPlaceholderReassignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v4/groups/{id}/placeholder_reassignments\n  method: post\n  operationId: postApiV4GroupsIdPlaceholderReassignments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/placeholder_reassignments/authorize\n  method: post\n  operationId: postApiV4GroupsIdPlaceholderReassignmentsAuthorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/variables\n  method: get\n  operationId: getApiV4GroupsIdVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/variables\n  method: post\n  operationId: postApiV4GroupsIdVariables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/variables/{key}\n  method: get\n  operationId: getApiV4GroupsIdVariablesKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/variables/{key}\n  method: put\n  operationId: putApiV4GroupsIdVariablesKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/variables/{key}\n  method: delete\n  operationId: deleteApiV4GroupsIdVariablesKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/integrations\n  method: get\n  operationId: getApiV4GroupsIdIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/groups/{id}/integrations/apple-app-store\n  method: put\n  operationId: putApiV4GroupsIdIntegrationsAppleAppStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/integrations/asana\n  method: put\n  operationId: putApiV4GroupsIdIntegrationsAsana\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/groups/{id}/integrations/assembla\n  method: put\n  operationId: putApiV4GroupsIdIntegrationsAssembla\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \n\n# --- truncated at 32 KB (378 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/gitlab-ci/refs/heads/main/agentic-access/gitlab-ci-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitlab-ci/refs/heads/main/agentic-access/gitlab-ci-agentic-access.yml
summary_line: 1125 operations · 627 acting · 22 human-in-the-loop
tags:
- DevOps
- CI/CD
- Pipelines
- GitLab
- DevSecOps
- Runners
- Container Registry
---
