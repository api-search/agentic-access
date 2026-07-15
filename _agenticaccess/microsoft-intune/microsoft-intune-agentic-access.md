---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 6
consequence_counts:
  read: 6
  safety-critical: 2
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Intune Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /deviceManagement/managedDevices/{managedDeviceId}/rebootNow
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /deviceManagement/managedDevices/{managedDeviceId}/resetPasscode
operation_count: 22
overview: 'Microsoft Intune exposes 22 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 14 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Intune
provider_slug: microsoft-intune
slug: microsoft-intune-agentic-access
source_filename: microsoft-intune-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-intune-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 6\n    acting: 16\n  by_consequence:\n    read: 6\n    write: 14\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /deviceManagement/managedDevices\n  method: get\n  operationId: listManagedDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - DeviceManagementManagedDevices.Read.All\n    - DeviceManagementManagedDevices.ReadWrite.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deviceManagement/managedDevices\n  method: post\n  operationId: createManagedDevice\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementManagedDevices.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/managedDevices/{managedDeviceId}\n  method: get\n  operationId: getManagedDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - DeviceManagementManagedDevices.Read.All\n    - DeviceManagementManagedDevices.ReadWrite.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deviceManagement/managedDevices/{managedDeviceId}\n  method: patch\n  operationId: updateManagedDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementManagedDevices.ReadWrite.All\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/managedDevices/{managedDeviceId}\n  method: delete\n  operationId: deleteManagedDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementManagedDevices.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/managedDevices/{managedDeviceId}/retire\n  method: post\n  operationId: retireManagedDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementManagedDevices.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/managedDevices/{managedDeviceId}/wipe\n  method: post\n  operationId: wipeManagedDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementManagedDevices.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/managedDevices/{managedDeviceId}/syncDevice\n  method: post\n  operationId: syncManagedDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementManagedDevices.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /deviceManagement/managedDevices/{managedDeviceId}/remoteLock\n  method: post\n  operationId: remoteLockManagedDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementManagedDevices.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/managedDevices/{managedDeviceId}/resetPasscode\n  method: post\n  operationId: resetPasscodeManagedDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - DeviceManagementManagedDevices.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /deviceManagement/managedDevices/{managedDeviceId}/rebootNow\n\
  \  method: post\n  operationId: rebootManagedDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - DeviceManagementManagedDevices.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /deviceManagement/deviceConfigurations\n  method: get\n  operationId: listDeviceConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - DeviceManagementConfiguration.Read.All\n    - DeviceManagementConfiguration.ReadWrite.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deviceManagement/deviceConfigurations/{deviceConfigurationId}\n  method: get\n  operationId: getDeviceConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - DeviceManagementConfiguration.Read.All\n    - DeviceManagementConfiguration.ReadWrite.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deviceManagement/deviceConfigurations/{deviceConfigurationId}\n  method: patch\n  operationId: updateDeviceConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementConfiguration.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/deviceConfigurations/{deviceConfigurationId}\n  method: delete\n  operationId: deleteDeviceConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementConfiguration.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign\n  method: post\n  operationId: assignDeviceConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementConfiguration.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/deviceCompliancePolicies\n  method: get\n  operationId: listDeviceCompliancePolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - DeviceManagementConfiguration.Read.All\n    - DeviceManagementConfiguration.ReadWrite.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}\n\
  \  method: get\n  operationId: getDeviceCompliancePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - DeviceManagementConfiguration.Read.All\n    - DeviceManagementConfiguration.ReadWrite.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}\n  method: patch\n  operationId: updateDeviceCompliancePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementConfiguration.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}\n  method: delete\n  operationId: deleteDeviceCompliancePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - DeviceManagementConfiguration.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign\n  method: post\n  operationId: assignDeviceCompliancePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - DeviceManagementConfiguration.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules\n  method: post\n  operationId: scheduleActionsForRules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - DeviceManagementConfiguration.ReadWrite.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-intune/refs/heads/main/agentic-access/microsoft-intune-agentic-access.yml
summary_line: 22 operations · 16 acting · 2 human-in-the-loop
tags:
- App Protection
- Azure
- Compliance
- Device Configuration
- Endpoint Management
- Enrollment
- MAM
- MDM
- Microsoft Graph
- Mobile Application Management
- Mobile Device Management
- Security
---
