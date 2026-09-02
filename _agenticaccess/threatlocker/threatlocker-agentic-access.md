---
acting_count: 46
action_class_counts:
  acting: 46
  connected: 37
api_specs:
- filename: threatlocker-actionlog-api-openapi.yml
  format: yaml
  label: ThreatLocker Action Log API
  slug: threatlocker-actionlog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-actionlog-api-openapi.yml
- filename: threatlocker-application-api-openapi.yml
  format: yaml
  label: ThreatLocker Application API
  slug: threatlocker-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-application-api-openapi.yml
- filename: threatlocker-approvalrequest-api-openapi.yml
  format: yaml
  label: ThreatLocker Approval Request API
  slug: threatlocker-approvalrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-approvalrequest-api-openapi.yml
- filename: threatlocker-computer-api-openapi.yml
  format: yaml
  label: ThreatLocker Computer API
  slug: threatlocker-computer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-computer-api-openapi.yml
- filename: threatlocker-computercheckin-api-openapi.yml
  format: yaml
  label: ThreatLocker Computer Checkin API
  slug: threatlocker-computercheckin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-computercheckin-api-openapi.yml
- filename: threatlocker-computergroup-api-openapi.yml
  format: yaml
  label: ThreatLocker Computer Group API
  slug: threatlocker-computergroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-computergroup-api-openapi.yml
- filename: threatlocker-maintenancemode-api-openapi.yml
  format: yaml
  label: ThreatLocker Maintenance Mode API
  slug: threatlocker-maintenancemode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-maintenancemode-api-openapi.yml
- filename: threatlocker-onlinedevices-api-openapi.yml
  format: yaml
  label: ThreatLocker Online Devices API
  slug: threatlocker-onlinedevices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-onlinedevices-api-openapi.yml
- filename: threatlocker-organization-api-openapi.yml
  format: yaml
  label: ThreatLocker Organization API
  slug: threatlocker-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-organization-api-openapi.yml
- filename: threatlocker-policy-api-openapi.yml
  format: yaml
  label: ThreatLocker Policy API
  slug: threatlocker-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-policy-api-openapi.yml
- filename: threatlocker-report-api-openapi.yml
  format: yaml
  label: ThreatLocker Report API
  slug: threatlocker-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-report-api-openapi.yml
- filename: threatlocker-savesearch-api-openapi.yml
  format: yaml
  label: ThreatLocker Save Search API
  slug: threatlocker-savesearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-savesearch-api-openapi.yml
- filename: threatlocker-scheduledagentaction-api-openapi.yml
  format: yaml
  label: ThreatLocker Scheduled Agent Action API
  slug: threatlocker-scheduledagentaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-scheduledagentaction-api-openapi.yml
- filename: threatlocker-systemaudit-api-openapi.yml
  format: yaml
  label: ThreatLocker System Audit API
  slug: threatlocker-systemaudit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-systemaudit-api-openapi.yml
- filename: threatlocker-tag-api-openapi.yml
  format: yaml
  label: ThreatLocker Tag API
  slug: threatlocker-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-tag-api-openapi.yml
- filename: threatlocker-threatlockerversion-api-openapi.yml
  format: yaml
  label: ThreatLocker Threat Locker Version API
  slug: threatlocker-threatlockerversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-threatlockerversion-api-openapi.yml
- filename: threatlocker-uploadrequest-api-openapi.yml
  format: yaml
  label: ThreatLocker Upload Request API
  slug: threatlocker-uploadrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-uploadrequest-api-openapi.yml
- filename: threatlocker-vdihyperv-api-openapi.yml
  format: yaml
  label: ThreatLocker VDI Hyper V API
  slug: threatlocker-vdihyperv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-vdihyperv-api-openapi.yml
consequence_counts:
  physical: 1
  read: 37
  safety-critical: 1
  write: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Threatlocker Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /portalapi/Computer/ComputerDisableProtection
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portalapi/ApprovalRequest/ApprovalRequestUpdateForTakeOwnership
operation_count: 83
overview: 'ThreatLocker exposes 83 API operations that an AI agent could call, of which 46 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 44 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ThreatLocker
provider_slug: threatlocker
slug: threatlocker-agentic-access
source_filename: threatlocker-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/threatlocker-portal-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 83\n  by_action_class:\n    acting: 46\n    connected: 37\n  by_consequence:\n    write: 44\n    read: 37\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /portalapi/ActionLog/ActionLogGetByParametersV2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ActionLog/ActionLogGetAllForFileHistory\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ActionLog/ActionLogGetAllForFileHistoryV2\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ActionLog/ActionLogGetById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ActionLog/ActionLogGetByIdV2\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ActionLog/ActionLogGetTestingEnvironmentDetailsById\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ActionLog/ActionLogGetPolicyConditionsForPermitApplication\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ActionLog/ActionLogGetSearchString\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ActionLog/ActionLogGetFileDownloadDetailsById\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Application/ApplicationGetById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Application/ApplicationGetForNetworkPolicyProcessById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Application/ApplicationGetResearchDetailsById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Application/ApplicationGetForMaintenanceMode\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /portalapi/Application/ApplicationGetMatchingList\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Application/ApplicationGetForApplicationOptions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ApprovalRequest/ApprovalRequestGetById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ApprovalRequest/ApprovalRequestGetFileDownloadDetailsById\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ApprovalRequest/ApprovalRequestGetPermitApplicationById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ApprovalRequest/ApprovalRequestPermitApplication\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ApprovalRequest/ApprovalRequestGetStorageApprovalById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /portalapi/ApprovalRequest/ApprovalRequestPermitStorageApproval\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ApprovalRequest/ApprovalRequestGetByParameters\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ApprovalRequest/ApprovalRequestGetCount\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ApprovalRequest/ApprovalRequestUpdateForTakeOwnership\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ApprovalRequest/ApprovalRequestUpdateForIgnore\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ApprovalRequest/ApprovalRequestUpdateForReject\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ApprovalRequest/ApprovalRequestAuthorizeForPermitById\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerGetByAllParameters\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerGetForEditById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Computer/ComputerUpdateForEdit\n\
  \  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerUpdateBaselineRescan\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerUpdateShouldRestartByIds\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /portalapi/Computer/ComputerUpdateShouldRestartByOrganization\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerMoveToOtherOrganization\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerEnableProtection\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerDisableProtection\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /portalapi/Computer/ComputerRemoveDuplicate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerUpdateMaintenanceMode\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerUpdateThreatlockerVersionByIds\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerGetThreatlockerVersions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Computer/ComputerUpdateToFinishMaintenanceMode\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerGetForNewComputer\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Computer/ComputerGetDownload\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerGetOSTypeByIds\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Computer/ComputerSignedScriptDownload\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Computer/ComputerSamplePathDownload\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Computer/ComputerUnSignedScriptDownload\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Computer/ComputerUpdateChannel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ComputerCheckin/ComputerCheckinGetByParameters\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ComputerGroup/ComputerGroupGetGroupAndComputer\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ComputerGroup/ComputerGroupGetDropdownByOrganizationId\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ComputerGroup/ComputerGroupGetForPermitApplication\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ComputerGroup/ComputerGroupGetForDownload\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/MaintenanceMode/MaintenanceModeGetByComputerId\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/MaintenanceMode/MaintenanceModeInsert\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/MaintenanceMode/MaintenanceModeEndById\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/MaintenanceMode/MaintenanceModeUpdateEndDateTimeForSpecificDate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/OnlineDevices/OnlineDevicesGetByParameters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Organization/OrganizationGetAuthKeyById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Organization/OrganizationUpdateAuthKeyById\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Organization/OrganizationGetForMoveComputers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Policy/PolicyGetById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Report/ReportGetByOrganizationId\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Report/ReportGetDynamicData\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/SaveSearch/SaveSearchGetByPage\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/SaveSearch/SaveSearchInsert\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/SaveSearch/SaveSearchDeleteById\n  method: delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ScheduledAgentAction/List\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ScheduledAgentAction/AppliesTo\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ScheduledAgentAction/GetForHydration\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/ScheduledAgentAction/GetByParameters\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ScheduledAgentAction\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ScheduledAgentAction/Abort\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/SystemAudit/SystemAuditGetForHealthCenter\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/SystemAudit/SystemAuditGetLoginAttemptFiltersForHealthCenter\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/SystemAudit/SystemAuditGetByParameters\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/Tag/TagGetById\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Tag/TagGetDowndownOptionsByOrganizationId\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/Tag/TagUpdate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/ThreatLockerVersion/ThreatLockerVersionGetForDropdownList\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portalapi/UploadRequest/UploadRequestInsert\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/UploadRequest/UploadRequestGet\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portalapi/VDIHyperV/VDIHyperVGetTestingEnvironmentDetails\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/agentic-access/threatlocker-agentic-access.yml
summary_line: 83 operations · 46 acting · 1 human-in-the-loop
tags:
- Cybersecurity
- Zero Trust
- Endpoint Security
- Application-Control
- allowlisting
- Ransomware Prevention
- Privileged Access Management
- Network Access Control
- Managed Detection and Response
- Device Management
- MSP
- Compliance
---
