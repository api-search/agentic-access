---
acting_count: 571
action_class_counts:
  acting: 571
  connected: 324
api_specs:
- filename: yugabytedb-aeon-openapi.yml
  format: yaml
  label: YugabyteDB Aeon REST API
  slug: aeon
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/openapi/yugabytedb-aeon-openapi.yml
- filename: yugabytedb-anywhere-v1-universes.yaml
  format: yaml
  label: YugabyteDB Anywhere REST API
  slug: anywhere
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/openapi/yugabytedb-anywhere-v1-universes.yaml
consequence_counts:
  physical: 4
  read: 324
  safety-critical: 33
  write: 534
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 33
kind: agentic-access
layout: agentic-access
method: generated
name: Yugabytedb Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/backups/{backupUUID}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/backups/{backupUUID}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/releases
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/releases
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/customers/{cUUID}/releases/{name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/customers/{cUUID}/releases/{name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/customers/{cUUID}/releases/{name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/customers/{cUUID}/releases/{name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/customers/{cUUID}/reset_password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/customers/{cUUID}/reset_password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/setup_universe_2dc
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/setup_universe_2dc
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/slow_queries
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/slow_queries
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/upgrade/kubernetes_overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/upgrade/kubernetes_overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/upgrade/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/upgrade/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/ybc/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/ybc/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/ybc_throttle_params
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/ybc_throttle_params
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/ybc_throttle_params_async
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/universes/{uniUUID}/ybc_throttle_params_async
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/customers/{cUUID}/validate_kubernetes_overrides
operation_count: 895
overview: 'YugabyteDB exposes 895 API operations that an AI agent could call, of which 571 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 324 read, 534 write, 4 physical, and 33 safety-critical.


  33 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: YugabyteDB
provider_slug: yugabytedb
slug: yugabytedb-agentic-access
source_filename: yugabytedb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/yugabytedb-aeon-openapi.yml, openapi/yugabytedb-anywhere-v1-alerts-monitoring.yaml,\n  openapi/yugabytedb-anywhere-v1-backups-restore.yaml, openapi/yugabytedb-anywhere-v1-full.yaml,\n  openapi/yugabytedb-anywhere-v1-high-availability.yaml, openapi/yugabytedb-anywhere-v1-providers-infra.yaml,\n  openapi/yugabytedb-anywhere-v1-releases-maintenance.yaml, openapi/yugabytedb-anywhere-v1-universes.yaml,\n  openapi/yugabytedb-anywhere-v1-users-rbac.yaml, openapi/yugabytedb-anywhere-v2-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 895\n  by_action_class:\n    connected: 324\n    acting: 571\n  by_consequence:\n    read: 324\n    write: 534\n    physical: 4\n    safety-critical:\
  \ 33\n  human_in_the_loop_required: 33\noperations:\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/projects/{projectId}/clusters\n  method: get\n  operationId: listClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/projects/{projectId}/clusters\n\
  \  method: post\n  operationId: createCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}\n  method: put\n  operationId: updateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}\n\
  \  method: delete\n  operationId: deleteCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/pause\n  method: post\n  operationId: pauseCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/resume\n  method: post\n  operationId: resumeCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/read-replicas\n  method: get\n  operationId: listReadReplicas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/read-replicas\n  method: post\n  operationId: createReadReplica\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/read-replicas\n  method: delete\n  operationId: deleteReadReplica\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/backups\n  method: get\n  operationId: listBackups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/backups\n  method: post\n  operationId: createBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/backups/{backupId}/restore\n\
  \  method: post\n  operationId: restoreBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/allow-lists\n  method: get\n  operationId: listAllowLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/projects/{projectId}/allow-lists\n  method: post\n  operationId: createAllowList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/allow-lists/{allowListId}\n\
  \  method: get\n  operationId: getAllowList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/projects/{projectId}/allow-lists/{allowListId}\n  method: delete\n  operationId: deleteAllowList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/maintenance-windows\n  method: get\n  operationId: getMaintenanceWindow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/projects/{projectId}/clusters/{clusterId}/maintenance-windows\n  method: put\n  operationId:\
  \ updateMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audit_logging_config\n  method: post\n  operationId: setAuditLoggingSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_channel_templates\n  method: get\n  operationId: listAlertChannelTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alert_channel_templates/{acType}\n\
  \  method: delete\n  operationId: deleteAlertChannelTemplates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_channel_templates/{acType}\n  method: get\n  operationId: getAlertChannelTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alert_channel_templates/{acType}\n  method: post\n  operationId: setAlertChannelTemplates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/customers/{cUUID}/alert_channels\n  method: get\n  operationId: listAlertChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alert_channels\n  method: post\n  operationId: createAlertChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_channels/{acUUID}\n  method: delete\n  operationId: deleteAlertChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/customers/{cUUID}/alert_channels/{acUUID}\n  method: get\n  operationId: getAlertChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alert_channels/{acUUID}\n  method: put\n  operationId: updateAlertChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_configurations\n  method: post\n  operationId: createAlertConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_configurations/list\n  method: post\n  operationId: listAlertConfigurations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_configurations/page\n  method: post\n  operationId: pageAlertConfigurations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_configurations/{configurationUUID}\n  method: delete\n  operationId: deleteAlertConfiguration\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_configurations/{configurationUUID}\n  method: get\n  operationId: getAlertConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alert_configurations/{configurationUUID}\n  method: put\n  operationId: updateAlertConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_configurations/{configurationUUID}/test_alert\n\
  \  method: post\n  operationId: sendTestAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_destinations\n  method: get\n  operationId: listAlertDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alert_destinations\n  method: post\n  operationId: createAlertDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/v1/customers/{cUUID}/alert_destinations/{adUUID}\n  method: delete\n  operationId: deleteAlertDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_destinations/{adUUID}\n  method: get\n  operationId: getAlertDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alert_destinations/{adUUID}\n  method: put\n  operationId: updateAlertDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_notification_preview\n  method: post\n  operationId: alertNotificationPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_template_settings\n  method: get\n  operationId: listAlertTemplateSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alert_template_settings\n  method: put\n  operationId: editAlertTemplateSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_template_settings/{settingsUUID}\n  method: delete\n  operationId: deleteAlertTemplateSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_template_variables\n  method: get\n  operationId: listAlertTemplateVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alert_template_variables\n  method: put\n  operationId: editAlertTemplateVariables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_template_variables/{variableUUID}\n  method: delete\n  operationId: deleteAlertTemplateVariables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alert_templates\n  method: post\n  operationId: listAlertTemplates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alerts\n\
  \  method: get\n  operationId: listOfAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alerts/acknowledge\n  method: post\n  operationId: acknowledgeByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alerts/active\n  method: get\n  operationId: listActive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alerts/count\n  method: post\n  operationId: countAlerts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alerts/page\n  method: post\n  operationId: pageAlerts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/alerts/{alertUUID}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/alerts/{alertUUID}/acknowledge\n  method: post\n  operationId: acknowledge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/pa_collector\n  method: get\n  operationId: listAllPACollectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/pa_collector\n  method: post\n  operationId: createPACollector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/pa_collector/{paUUID}\n  method: delete\n  operationId: deletePACollector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/pa_collector/{paUUID}\n  method: get\n  operationId: getPACollector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/pa_collector/{paUUID}\n  method: put\n  operationId: editPACollector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/performance_recommendation_state_change/page\n  method: post\n  operationId: pageAuditInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/performance_recommendations\n  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/performance_recommendations/hide\n  method: post\n  operationId: hide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/performance_recommendations/page\n\
  \  method: post\n  operationId: page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/performance_recommendations/resolve\n  method: post\n  operationId: resolve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/performance_recommendations/{rUUID}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/tasks/{tUUID}/audit_info\n\
  \  method: get\n  operationId: getTaskAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/tasks/{tUUID}/audit_user\n  method: get\n  operationId: getUserFromTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/telemetry_provider\n  method: get\n  operationId: listAllTelemetryProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/telemetry_provider\n  method: post\n  operationId: createTelemetry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/telemetry_provider/{intUUID}\n  method: delete\n  operationId: deleteTelemetryProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/telemetry_provider/{intUUID}\n  method: get\n  operationId: getTelemetryProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/universes/{uUUID}/pa_collector\n  method: delete\n  operationId: unregisterUniverse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/universes/{uUUID}/pa_collector\n  method: get\n  operationId: checkRegistered\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/universes/{uUUID}/pa_collector/{paUUID}\n  method: put\n  operationId: registerUniverse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/universes/{uniUUID}/last_run\n  method: get\n  operationId: getLatestRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/universes/{uniUUID}/perf_advisor_settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/universes/{uniUUID}/perf_advisor_settings\n  method: post\n  operationId: updateSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/universes/{uniUUID}/start_manually\n  method: post\n  operationId: runPerfAdvisor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/users/{uUUID}/audit_trail\n  method: get\n  operationId: ListOfAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/grafana_dashboard\n  method: get\n  operationId: GrafanaDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/logging_config\n  method: post\n  operationId: setLoggingSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/prometheus_metrics\n  method: get\n  operationId: MetricsDetail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/backups\n  method: delete\n  operationId: deleteBackups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/backups\n  method: post\n  operationId: createbackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/backups/delete\n  method: post\n  operationId: deleteBackupsV2\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/backups/page\n  method: post\n  operationId: listBackupsV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/backups/{backupUUID}\n  method: get\n  operationId: getBackupV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/backups/{backupUUID}\n  method: put\n  operationId: editBackupV2\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/backups/{backupUUID}/list_increments\n  method: get\n  operationId: listIncrementalBackups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/backups/{backupUUID}/stop\n  method: post\n  operationId: stopBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/customers/{cUUID}/backups/{baseBackupUUID}/restorable_keyspace_tables\n\
  \  method: get\n  operationId: listRestorableKeyspaceTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/customers/{cUUID}/cloud/{cloud}/buckets\n  method: post\n  operationId: listBuckets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{cUUID}/configs\n  method: get\n  operationId: getListOfCustomerConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path\n\n# --- truncated at 32 KB (287 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/agentic-access/yugabytedb-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/agentic-access/yugabytedb-agentic-access.yml
summary_line: 895 operations · 571 acting · 33 human-in-the-loop
tags:
- Cloud Database
- Database
- DBaaS
- Distributed SQL
- PostgreSQL
---
