---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 21
api_specs:
- filename: cisco-expressway-configuration-api-openapi.yml
  format: yaml
  label: Cisco Expressway Configuration API
  slug: cisco-expressway-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-configuration-api-openapi.yml
- filename: cisco-expressway-status-api-openapi.yml
  format: yaml
  label: Cisco Expressway Status API
  slug: cisco-expressway-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-status-api-openapi.yml
consequence_counts:
  physical: 23
  read: 21
  safety-critical: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Cisco Expressway Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /provisioning/controller/zone/traversalclient
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /provisioning/controller/zone/traversalclient
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /provisioning/controller/zone/traversalclient
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provisioning/common/searchrule
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /provisioning/common/searchrule
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /provisioning/common/searchrule
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /provisioning/common/sip/configuration
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provisioning/common/transform
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /provisioning/common/transform
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /provisioning/common/transform
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provisioning/common/zone/dns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provisioning/common/zone/neighbor
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /provisioning/common/zone/neighbor
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /provisioning/common/zone/neighbor
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provisioning/edge/zone/traversalserver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /provisioning/edge/zone/traversalserver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /provisioning/edge/zone/traversalserver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/provisioning/common/adminaccount/changepassword
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/provisioning/common/dns/dnsserver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/provisioning/common/dns/dnsserver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/provisioning/common/dns/dnsserver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/provisioning/common/sftpconfig
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/provisioning/common/time/ntpserver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/provisioning/common/time/ntpserver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/provisioning/common/time/ntpserver
operation_count: 47
overview: 'Cisco Expressway exposes 47 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 23 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cisco Expressway
provider_slug: cisco-expressway
slug: cisco-expressway-agentic-access
source_filename: cisco-expressway-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cisco-expressway-configuration-api-openapi.yml, openapi/cisco-expressway-status-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 21\n    acting: 26\n  by_consequence:\n    read: 21\n    physical: 23\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /provisioning/common/sysinfo\n  method: get\n  operationId: getSystemInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provisioning/common/dns/dnsserver\n  method: get\n  operationId: listDnsServers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provisioning/common/dns/dnsserver\n  method: post\n  operationId: createDnsServer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/provisioning/common/dns/dnsserver\n  method: put\n  operationId: updateDnsServer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/provisioning/common/dns/dnsserver\n  method:\
  \ delete\n  operationId: deleteDnsServer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/provisioning/common/time/ntpserver\n  method: get\n  operationId: listNtpServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provisioning/common/time/ntpserver\n  method: post\n  operationId: createNtpServer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/provisioning/common/time/ntpserver\n  method: put\n  operationId: updateNtpServer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/provisioning/common/time/ntpserver\n  method: delete\n  operationId: deleteNtpServer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/provisioning/common/sftpconfig\n  method: get\n  operationId: getSftpConfig\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provisioning/common/sftpconfig\n  method: put\n  operationId: updateSftpConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/provisioning/common/upgrade\n  method: post\n  operationId: triggerUpgrade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/provisioning/common/adminaccount/changepassword\n\
  \  method: post\n  operationId: changeAdminPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/edge/zone/traversalserver\n  method: get\n  operationId: listEdgeTraversalServerZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/edge/zone/traversalserver\n  method: post\n  operationId: createEdgeTraversalServerZone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/edge/zone/traversalserver\n  method: put\n  operationId: updateEdgeTraversalServerZone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/edge/zone/traversalserver\n  method: delete\n  operationId: deleteEdgeTraversalServerZone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/controller/zone/traversalclient\n\
  \  method: get\n  operationId: listControllerTraversalClientZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/controller/zone/traversalclient\n  method: post\n  operationId: createControllerTraversalClientZone\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /provisioning/controller/zone/traversalclient\n  method: put\n  operationId: updateControllerTraversalClientZone\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /provisioning/controller/zone/traversalclient\n  method: delete\n  operationId: deleteControllerTraversalClientZone\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /provisioning/common/zone/neighbor\n  method: get\n  operationId: listNeighborZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/common/zone/neighbor\n  method: post\n  operationId: createNeighborZone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/common/zone/neighbor\n  method: put\n  operationId: updateNeighborZone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/common/zone/neighbor\n  method: delete\n  operationId: deleteNeighborZone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /provisioning/common/zone/dns\n  method: get\n  operationId: listDnsZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/common/zone/dns\n  method: post\n  operationId: createDnsZone\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/common/searchrule\n  method: get\n  operationId: listSearchRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/common/searchrule\n  method: post\n  operationId: createSearchRule\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/common/searchrule\n  method: put\n  operationId: updateSearchRule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/common/searchrule\n  method: delete\n  operationId: deleteSearchRule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    \
  \  exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/common/transform\n  method: get\n  operationId: listTransforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/common/transform\n  method: post\n  operationId: createTransform\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/common/transform\n  method: put\n  operationId: updateTransform\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/common/transform\n  method: delete\n  operationId: deleteTransform\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/common/sip/configuration\n  method: get\n  operationId: getSipConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/common/sip/configuration\n  method: put\n  operationId: updateSipConfiguration\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status/common/systeminfo\n  method: get\n  operationId: getSystemStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/common/alarms\n  method: get\n  operationId: listAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/common/calls\n  method: get\n  operationId: listActiveCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /status/common/callhistory\n  method: get\n  operationId: getCallHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/common/registrations\n  method: get\n  operationId: listRegistrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status/common/smartlicensing/licensing\n  method: get\n  operationId: getSmartLicensingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status/common/upgradestatus\n  method: get\n  operationId: getUpgradeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/common/zones\n  method: get\n  operationId:\
  \ listZoneStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/common/resourceusage\n  method: get\n  operationId: getResourceUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/common/turnrelays\n  method: get\n  operationId: listTurnRelays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/agentic-access/cisco-expressway-agentic-access.yml
summary_line: 47 operations · 26 acting · 3 human-in-the-loop
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
---
