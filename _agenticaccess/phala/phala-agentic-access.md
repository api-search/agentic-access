---
acting_count: 50
action_class_counts:
  acting: 50
  connected: 52
api_specs:
- filename: phala-apps-api-openapi.yml
  format: yaml
  label: Phala Network Apps API
  slug: phala-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-api-openapi.yml
- filename: phala-apps-kms-info-api-openapi.yml
  format: yaml
  label: Phala Network Apps Kms Info API
  slug: phala-apps-kms-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-kms-info-api-openapi.yml
- filename: phala-apps-pending-updates-api-openapi.yml
  format: yaml
  label: Phala Network Apps Pending Updates API
  slug: phala-apps-pending-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-pending-updates-api-openapi.yml
- filename: phala-attestations-api-openapi.yml
  format: yaml
  label: Phala Network Attestations API
  slug: phala-attestations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-attestations-api-openapi.yml
- filename: phala-cvms-api-openapi.yml
  format: yaml
  label: Phala Network CVMs API
  slug: phala-cvms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-cvms-api-openapi.yml
- filename: phala-cvms-network-config-api-openapi.yml
  format: yaml
  label: Phala Network Cvms Network Config API
  slug: phala-cvms-network-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-cvms-network-config-api-openapi.yml
- filename: phala-instance-types-api-openapi.yml
  format: yaml
  label: Phala Network Instance Types API
  slug: phala-instance-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-instance-types-api-openapi.yml
- filename: phala-kms-api-openapi.yml
  format: yaml
  label: Phala Network KMS API
  slug: phala-kms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-kms-api-openapi.yml
- filename: phala-ssh-keys-api-openapi.yml
  format: yaml
  label: Phala Network SSH Keys API
  slug: phala-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-ssh-keys-api-openapi.yml
- filename: phala-webhooks-api-openapi.yml
  format: yaml
  label: Phala Network Webhooks API
  slug: phala-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-webhooks-api-openapi.yml
consequence_counts:
  physical: 11
  read: 52
  safety-critical: 3
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Phala Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/cvms/batch-stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/cvms/{cvm_id}/shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/cvms/{cvm_id}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/apps/{app_id}/cvms/is-allowed
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/apps/{app_id}/is-allowed
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/apps/{app_id}/revisions/{revision_id}/redeploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/cvms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/cvms/eliza
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/cvms/provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/cvms/provision/eliza
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/cvms/{cvm_id}/compose_file/provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/cvms/{cvm_id}/revisions/{revision_id}/redeploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/workspace/webhooks/{webhook_id}/deliveries/{event_id}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/workspace/webhooks/{webhook_id}/test
operation_count: 102
overview: 'Phala Network exposes 102 API operations that an AI agent could call, of which 50 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 52 read, 36 write, 11 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Phala Network
provider_slug: phala
slug: phala-agentic-access
source_filename: phala-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/phala-cloud-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 102\n  by_action_class:\n    acting: 50\n    connected: 52\n  by_consequence:\n    physical: 11\n    write: 36\n    read: 52\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /api/v1/cvms/provision/eliza\n  method: post\n  operationId: handle_provision_cvm_for_eliza_api_v1_cvms_provision_eliza_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/cvms/provision\n  method: post\n  operationId: handle_provision_cvm_api_v1_cvms_provision_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/workload\n  method: post\n  operationId: handle_create_cvm_for_workload_api_v1_cvms_workload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms\n  method: post\n  operationId: handle_create_cvm_from_povision_api_v1_cvms_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms\n  method: get\n  operationId: handle_list_cvms_api_v1_cvms_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/eliza\n  method: post\n  operationId: handle_create_eliza_from_provision_api_v1_cvms_eliza_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/cvms/{cvm_id}/compose_file\n  method: get\n  operationId: get_cvm_compose_file_api_v1_cvms__cvm_id__compose_file_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/compose_file\n  method: patch\n  operationId: trigger_cvm_compose_file_update_api_v1_cvms__cvm_id__compose_file_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/compose_file\n  method: post\n  operationId: submit_cvm_compose_file_update_api_v1_cvms__cvm_id__compose_file_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/compose_file/provision\n  method: post\n  operationId: provision_for_cvm_compose_file_update_api_v1_cvms__cvm_id__compose_file_provision_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/replicas\n  method: post\n  operationId: handle_replicate_cvm_api_v1_cvms__cvm_id__replicas_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/cvms/{cvm_id}/operations\n  method: get\n  operationId: get_cvm_operations_api_v1_cvms__cvm_id__operations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/operations/cancel\n  method: post\n  operationId: cancel_cvm_operation_api_v1_cvms__cvm_id__operations_cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/docker-compose.yml\n  method: get\n  operationId: handle_get_cvm_docker_compose_api_v1_cvms__cvm_id__docker_compose_yml_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/cvms/{cvm_id}/pre-launch-script\n  method: get\n  operationId: handle_get_cvm_prelaunch_script_api_v1_cvms__cvm_id__pre_launch_script_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/pre-launch-script\n  method: patch\n  operationId: update_cvm_pre_launch_script_api_v1_cvms__cvm_id__pre_launch_script_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/available-os-images\n  method: get\n  operationId: get_available_os_images_api_v1_cvms__cvm_id__available_os_images_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/os-image\n  method: patch\n  operationId: update_cvm_os_image_api_v1_cvms__cvm_id__os_image_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/envs\n  method: patch\n  operationId: update_cvm_envs_api_v1_cvms__cvm_id__envs_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/docker-compose\n  method: patch\n  operationId: update_cvm_docker_compose_api_v1_cvms__cvm_id__docker_compose_patch\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/revisions/{revision_id}/redeploy\n  method: post\n  operationId: redeploy_cvm_revision_api_v1_cvms__cvm_id__revisions__revision_id__redeploy_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/instance-ids\n  method: patch\n  operationId: handle_batch_refresh_cvm_instance_ids_api_v1_cvms_instance_ids_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/paginated\n  method: get\n  operationId: handle_list_cvms_paginated_api_v1_cvms_paginated_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/instance-id\n  method: patch\n  operationId: handle_refresh_cvm_instance_id_api_v1_cvms__cvm_id__instance_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}\n  method: get\n  operationId: handle_get_cvm_api_v1_cvms__cvm_id__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}\n  method: delete\n  operationId: handle_remove_cvm_api_v1_cvms__cvm_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}\n  method: patch\n  operationId: update_cvm_endpoint_api_v1_cvms__cvm_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/stats\n  method: get\n  operationId: handle_get_cvm_stats_api_v1_cvms__cvm_id__stats_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/attestation\n  method: get\n  operationId: handle_get_cvm_attestation_api_v1_cvms__cvm_id__attestation_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/network\n  method: get\n  operationId: handle_get_cvm_network_info_api_v1_cvms__cvm_id__network_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/start\n  method: post\n  operationId: handle_start_cvm_api_v1_cvms__cvm_id__start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/shutdown\n  method: post\n  operationId: handle_shutdown_cvm_api_v1_cvms__cvm_id__shutdown_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/stop\n  method: post\n  operationId: handle_stop_cvm_api_v1_cvms__cvm_id__stop_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/restart\n\
  \  method: post\n  operationId: handle_restart_cvm_api_v1_cvms__cvm_id__restart_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/operation-status\n  method: get\n  operationId: get_operation_status_api_v1_cvms__cvm_id__operation_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/name\n  method: patch\n  operationId: handle_update_cvm_name_api_v1_cvms__cvm_id__name_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/listed\n  method: patch\n  operationId: handle_update_cvm_listed_api_v1_cvms__cvm_id__listed_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/scheduled-delete\n  method: patch\n  operationId: handle_update_cvm_scheduled_delete_api_v1_cvms__cvm_id__scheduled_delete_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/batch-stop\n  method: post\n  operationId: handle_batch_stop_cvms_api_v1_cvms_batch_stop_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/status/batch\n  method: post\n  operationId: handle_batch_cvm_status_api_v1_status_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/state\n  method: get\n  operationId: handle_get_cvm_state_api_v1_cvms__cvm_id__state_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/network-config\n\
  \  method: get\n  operationId: handle_get_network_config_api_v1_cvms__cvm_id__network_config_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/network-config\n  method: patch\n  operationId: handle_update_network_config_api_v1_cvms__cvm_id__network_config_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/ports\n  method: get\n  operationId: handle_get_port_mappings_api_v1_cvms__cvm_id__ports_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/ports\n  method: put\n  operationId:\
  \ handle_set_port_mappings_api_v1_cvms__cvm_id__ports_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/firewall-status\n  method: get\n  operationId: handle_get_firewall_status_api_v1_cvms__cvm_id__firewall_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/commit-update\n  method: get\n  operationId: get_commit_update_info_api_v1_cvms__cvm_id__commit_update_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cvms/{cvm_id}/commit-update\n  method: post\n  operationId: commit_cvm_update_api_v1_cvms__cvm_id__commit_update_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/commit-replica\n  method: post\n  operationId: commit_cvm_replica_api_v1_cvms__cvm_id__commit_replica_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/customize-domain-diagnose\n  method: post\n  operationId: diagnose_custom_domains_api_v1_cvms__cvm_id__customize_domain_diagnose_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cvms/{cvm_id}/user_config\n  method: get\n  operationId: get_cvm_user_config_api_v1_cvms__cvm_id__user_config_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kms\n  method: get\n  operationId: list_kms_api_v1_kms_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kms/{kms_id}\n  method: get\n  operationId: get_kms_info_api_v1_kms__kms_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kms/{kms_id}/pubkey/{app_id}\n  method: get\n  operationId: get_app_env_encrypt_pubkey_api_v1_kms__kms_id__pubkey__app_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kms/phala/next_app_id\n  method: get\n  operationId: get_next_app_id_api_v1_kms_phala_next_app_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kms/{kms_id}/info\n  method: get\n  operationId: inspect_kms_api_v1_kms__kms_id__info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kms/on-chain/{chain}\n  method: get\n  operationId: get_kms_onchain_detail_api_v1_kms_on_chain__chain__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps\n  method: get\n  operationId: list_dstack_apps_api_v1_apps_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/filter-options\n  method: get\n  operationId: get_filter_options_api_v1_apps_filter_options_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}\n  method: get\n  operationId: get_dstack_app_api_v1_apps__app_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/cvms\n  method: get\n  operationId: handle_get_app_cvms_api_v1_apps__app_id__cvms_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/cvms/{vm_uuid}/replicas\n  method: post\n  operationId:\
  \ handle_replicate_cvm_api_v1_apps__app_id__cvms__vm_uuid__replicas_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{app_id}/instances\n  method: post\n  operationId: handle_create_app_instance_api_v1_apps__app_id__instances_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{app_id}/device-allowlist\n  method: get\n  operationId: get_device_allowlist_api_v1_apps__app_id__device_allowlist_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/attestations\n  method: get\n  operationId: handle_get_app_attestation_api_v1_apps__app_id__attestations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/attestations/tcb-evaluation\n  method: get\n  operationId: handle_get_app_tcb_evaluation_api_v1_apps__app_id__attestations_tcb_evaluation_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/revisions\n  method: get\n  operationId: get_app_revisions_api_v1_apps__app_id__revisions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/revisions/{revision_id}\n  method: get\n  operationId:\
  \ get_app_revision_detail_api_v1_apps__app_id__revisions__revision_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/revisions/{revision_id}/redeploy\n  method: post\n  operationId: redeploy_app_revision_api_v1_apps__app_id__revisions__revision_id__redeploy_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{app_id}/usage\n  method: get\n  operationId: get_app_usage_api_v1_apps__app_id__usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/is-allowed\n\
  \  method: post\n  operationId: handle_app_is_allowed_api_v1_apps__app_id__is_allowed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{app_id}/cvms/is-allowed\n  method: post\n  operationId: handle_app_cvms_is_allowed_api_v1_apps__app_id__cvms_is_allowed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{app_id}/kms-info\n  method: get\n  operationId: get_app_kms_info_api_v1_apps__app_id__kms_info_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/pending-updates\n  method: get\n  operationId: get_pending_updates_api_v1_apps__app_id__pending_updates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app_id}/pending-updates/{vm_uuid}/{compose_hash}/preview\n  method: get\n  operationId: get_pending_update_preview_api_v1_apps__app_id__pending_updates__vm_uuid___compose_hash__preview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/instance-types\n  method: get\n  operationId: list_all_families_api_v1_instance_types_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/instance-types/{family}\n  method: get\n  operationId: list_family_instance_types_api_v1_instance_types__family__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attestations/verify\n  method: post\n  operationId: handle_upload_and_verify_api_v1_attestations_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/attestations/recent\n  method: get\n  operationId: handle_list_recent_api_v1_attestations_recent_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attestations/view/{checksum}\n\
  \  method: get\n  operationId: handle_view_api_v1_attestations_view__checksum__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attestations/collateral/{checksum}\n  method: get\n  operationId: get_collateral_api_v1_attestations_collateral__checksum__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attestations/raw/{checksum}\n  method: get\n  operationId: handle_get_raw_api_v1_attestations_raw__checksum__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attestations/raw/{checksum}\n  method: head\n  operationId: handle_check_raw_file_api_v1_attestations_raw__checksum__head\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attestations/ppids\n  method: get\n  operationId: handle_list_ppids_api_v1_attestations_ppids_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attestations/device_ids\n  method: get\n  operationId: handle_list_device_ids_api_v1_attestations_device_ids_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attestations/nodes\n  method: get\n  operationId: handle_list_nodes_api_v1_attestations_nodes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/webhooks\n  method: get\n  operationId: list_webhooks_api_v1_workspace_webhooks_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/webhooks\n  method: post\n  operationId: create_webhook_api_v1_workspace_webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspace/webhooks/{webhook_id}\n  method: get\n  operationId: get_webhook_api_v1_workspace_webhooks__webhook_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/webhooks/{webhook_id}\n  method: put\n  operationId: update_webhook_api_v1_workspace_webhooks__webhook_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspace/webhooks/{webhook_id}\n  method: delete\n  operationId: delete_webhook_api_v1_workspace_webhooks__webhook_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspace/webhooks/{webhook_id}/reveal-secret\n  method: post\n  operationId: reveal_webhook_secret_api_v1_workspace_webhooks__webhook_id__reveal_secret_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspace/webhooks/{webhook_id}/rotate-secret\n  method: post\n  operationId: rotate_webhook_secret_api_v1_workspace_webhooks__webhook_id__rotate_secret_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workspace/webhooks/{webhook_id}/test\n  method: post\n  operationId: test_webhook_api_v1_workspace_webhooks__webhook_id__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/workspace/webhooks/{webhook_id}/deliveries\n  method: get\n  operationId: list_deliveries_api_v1_workspace_webhooks__webhook_id__deliveries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (34 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/agentic-access/phala-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/agentic-access/phala-agentic-access.yml
summary_line: 102 operations · 50 acting · 3 human-in-the-loop
tags:
- Company
- Confidential Computing
- Trusted Execution Environments
- Inference
- Cloud Infrastructure
- Attestation
- LLM Router
---
