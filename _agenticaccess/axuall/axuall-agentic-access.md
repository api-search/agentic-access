---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 29
api_specs:
- filename: axuall-actor-api-openapi.yml
  format: yaml
  label: Axuall Actor API
  slug: axuall-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-actor-api-openapi.yml
- filename: axuall-address-deduplications-api-openapi.yml
  format: yaml
  label: Axuall Address Deduplications API
  slug: axuall-address-deduplications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-address-deduplications-api-openapi.yml
- filename: axuall-agent-api-openapi.yml
  format: yaml
  label: Axuall Agent API
  slug: axuall-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-agent-api-openapi.yml
- filename: axuall-authentication-api-openapi.yml
  format: yaml
  label: Axuall Authentication API
  slug: axuall-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-authentication-api-openapi.yml
- filename: axuall-case-log-artifact-api-openapi.yml
  format: yaml
  label: Axuall Case Log Artifact API
  slug: axuall-case-log-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-case-log-artifact-api-openapi.yml
- filename: axuall-documents-api-openapi.yml
  format: yaml
  label: Axuall Documents API
  slug: axuall-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-documents-api-openapi.yml
- filename: axuall-email-api-openapi.yml
  format: yaml
  label: Axuall Email API
  slug: axuall-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-email-api-openapi.yml
- filename: axuall-facilities-api-openapi.yml
  format: yaml
  label: Axuall Facilities API
  slug: axuall-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-facilities-api-openapi.yml
- filename: axuall-fsmb-artifact-api-openapi.yml
  format: yaml
  label: Axuall FSMB Artifact API
  slug: axuall-fsmb-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-fsmb-artifact-api-openapi.yml
- filename: axuall-invite-api-openapi.yml
  format: yaml
  label: Axuall Invite API
  slug: axuall-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-invite-api-openapi.yml
- filename: axuall-monitoring-reports-api-openapi.yml
  format: yaml
  label: Axuall Monitoring reports API
  slug: axuall-monitoring-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-monitoring-reports-api-openapi.yml
- filename: axuall-provider-preview-api-openapi.yml
  format: yaml
  label: Axuall Provider Preview API
  slug: axuall-provider-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-provider-preview-api-openapi.yml
- filename: axuall-providers-api-openapi.yml
  format: yaml
  label: Axuall Providers API
  slug: axuall-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-providers-api-openapi.yml
- filename: axuall-recipes-api-openapi.yml
  format: yaml
  label: Axuall Recipes API
  slug: axuall-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-recipes-api-openapi.yml
- filename: axuall-tasks-api-openapi.yml
  format: yaml
  label: Axuall Tasks API
  slug: axuall-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/openapi/axuall-tasks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 29
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Axuall Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/agent/chat
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/send_invite
operation_count: 43
overview: 'Axuall exposes 43 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 12 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Axuall
provider_slug: axuall
slug: axuall-agentic-access
source_filename: axuall-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: generated\nsource: openapi/axuall-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 29\n    acting: 14\n  by_consequence:\n    read: 29\n    write: 12\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/current_actor\n  method: get\n  operationId: get_current_actor_v2_current_actor_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/email/inbound\n  method: post\n  operationId: email_inbound_v2_email_inbound_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/verification-emails/inbound\n  method: post\n  operationId: verification_email_inbound_v2_verification_emails_inbound_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/agent/chat\n  method: post\n  operationId: agent_chat_v2_agent_chat_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v2/agent/suggest-prompts\n  method: get\n  operationId: list_agent_suggest_prompts_v2_agent_suggest_prompts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/agent/conversations\n  method: get\n  operationId: list_agent_conversations_v2_agent_conversations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/agent/task/{task_id}\n  method: get\n  operationId: get_agent_task_status_v2_agent_task__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/agent/conversations/{conversation_id}/messages\n  method: get\n  operationId: get_agent_conversation_messages_v2_agent_conversations__conversation_id__messages_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/agent/conversations/{conversation_id}/messages/{message_id}/feedback\n  method: post\n  operationId: post_agent_message_feedback_v2_agent_conversations__conversation_id__messages__message_id__feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/app_req_list\n  method: get\n  operationId: list_application_requirements_v2_app_req_list_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth\n  method: post\n  operationId: authenticate_user_v2_auth_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sso\n  method: get\n  operationId: sso_initiation_v2_sso_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/case_logs/{npi}/{type}\n  method: get\n  operationId: get_case_log_artifact_v2_case_logs__npi___type__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/{npi}/{type}\n  method: get\n  operationId: get_document_artifact_v2_documents__npi___type__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/facility_list\n  method:\
  \ get\n  operationId: list_facilities_v2_facility_list_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/fsmb/artifact\n  method: get\n  operationId: get_fsmb_artifact_v2_fsmb_artifact_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/invite\n  method: post\n  operationId: create_invite_v2_invite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/send_invite\n  method: post\n  operationId: send_invite_v2_send_invite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/provider_preview\n  method: get\n  operationId: provider_preview_v2_provider_preview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/provider_prefill\n  method: get\n  operationId: provider_prefill_v2_provider_prefill_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/providers\n  method: get\n  operationId: list_providers_v2_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/providers\n  method: post\n  operationId:\
  \ register_provider_v2_providers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/providers/{provider_id}\n  method: get\n  operationId: get_provider_v2_providers__provider_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/providers/{provider_id}/files\n  method: get\n  operationId: list_provider_files_v2_providers__provider_id__files_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/providers/{provider_id}/verified_share\n  method: get\n  operationId: get_provider_verified_share_v2_providers__provider_id__verified_share_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/providers/{provider_id}/changes\n  method: get\n  operationId: list_provider_credential_changes_v2_providers__provider_id__changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/providers/{provider_id}/assign_task\n  method: post\n  operationId: assign_task_v2_providers__provider_id__assign_task_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/providers/{provider_id}/cancel_task\n  method: post\n  operationId: cancel_task_v2_providers__provider_id__cancel_task_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/providers/{provider_id}/workflows\n  method: post\n  operationId: assign_workflow_v2_providers__provider_id__workflows_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/providers/{provider_id}/deactivation\n  method: post\n  operationId: deactivate_clinician_v2_providers__provider_id__deactivation_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/providers/{provider_id}/attested_reqirements\n  method: get\n  operationId: list_attested_requirements_v2_providers__provider_id__attested_reqirements_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/providers/{provider_id}/facilities\n  method: get\n  operationId: list_provider_facilities_v2_providers__provider_id__facilities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/providers/{provider_id}/facilities\n  method: post\n  operationId: enroll_provider_v2_providers__provider_id__facilities_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/task_sets\n  method: get\n  operationId: list_task_sets_v2_task_sets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks\n  method: get\n  operationId: List_Tasks_v2_tasks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assigned_tasks\n  method: get\n  operationId: list_assigned_tasks_v2_assigned_tasks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitoring/dimensions\n  method: get\n  operationId: list_dimensions_v2_monitoring_dimensions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitoring/dimensions/credential\n  method: get\n  operationId: get_credential_dimension_v2_monitoring_dimensions_credential_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitoring/dimensions/{dimension_name}\n  method: get\n  operationId: get_dimension_v2_monitoring_dimensions__dimension_name__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitoring/findings\n  method: get\n  operationId: list_findings_v2_monitoring_findings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitoring/expirables\n  method: get\n  operationId: list_expirables_v2_monitoring_expirables_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/address_deduplications\n  method: post\n  operationId: create_address_deduplication_v2_address_deduplications_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/address_deduplications/{task_id}\n  method: get\n  operationId: get_address_deduplication_v2_address_deduplications__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axuall/refs/heads/main/agentic-access/axuall-agentic-access.yml
summary_line: 43 operations · 14 acting
tags:
- Company
- Healthcare
- Data
- Credentialing
- AI
---
