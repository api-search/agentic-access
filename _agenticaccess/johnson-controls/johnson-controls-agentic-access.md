---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 54
api_specs:
- filename: johnson-controls-activities-api-openapi.yml
  format: yaml
  label: Johnson Controls Activities API
  slug: johnson-controls-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-activities-api-openapi.yml
- filename: johnson-controls-alarms-api-openapi.yml
  format: yaml
  label: Johnson Controls Alarms API
  slug: johnson-controls-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-alarms-api-openapi.yml
- filename: johnson-controls-audits-api-openapi.yml
  format: yaml
  label: Johnson Controls Audits API
  slug: johnson-controls-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-audits-api-openapi.yml
- filename: johnson-controls-authentication-api-openapi.yml
  format: yaml
  label: Johnson Controls Authentication API
  slug: johnson-controls-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-authentication-api-openapi.yml
- filename: johnson-controls-equipment-api-openapi.yml
  format: yaml
  label: Johnson Controls Equipment API
  slug: johnson-controls-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-equipment-api-openapi.yml
- filename: johnson-controls-network-devices-api-openapi.yml
  format: yaml
  label: Johnson Controls network devices API
  slug: johnson-controls-network-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-network-devices-api-openapi.yml
- filename: johnson-controls-objects-api-openapi.yml
  format: yaml
  label: Johnson Controls Objects API
  slug: johnson-controls-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-objects-api-openapi.yml
- filename: johnson-controls-schemas-api-openapi.yml
  format: yaml
  label: Johnson Controls Schemas API
  slug: johnson-controls-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-schemas-api-openapi.yml
- filename: johnson-controls-spaces-api-openapi.yml
  format: yaml
  label: Johnson Controls Spaces API
  slug: johnson-controls-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-spaces-api-openapi.yml
- filename: johnson-controls-streaming-api-openapi.yml
  format: yaml
  label: Johnson Controls Streaming API
  slug: johnson-controls-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-streaming-api-openapi.yml
- filename: johnson-controls-time-series-api-openapi.yml
  format: yaml
  label: Johnson Controls time series API
  slug: johnson-controls-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-time-series-api-openapi.yml
consequence_counts:
  physical: 1
  read: 54
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Johnson Controls Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /objects/{objectId}/commands/{commandId}
operation_count: 70
overview: 'Johnson Controls exposes 70 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 54 read, 15 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Johnson Controls
provider_slug: johnson-controls
slug: johnson-controls-agentic-access
source_filename: johnson-controls-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/johnson-controls-metasys-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 70\n  by_action_class:\n    acting: 16\n    connected: 54\n  by_consequence:\n    write: 15\n    read: 54\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /login\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refreshToken\n  method: get\n  operationId: getToken\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities\n  method: get\n  operationId: getActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities/batch\n  method: post\n  operationId: postActivitiesBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activities/streams/{streamId}/subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteActivitiesSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects\n  method: get\n  operationId: getObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects\n  method: post\n  operationId: postObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectId}/objects\n  method: get\n  operationId: getChildObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objectIdentifiers\n  method: get\n  operationId: getObjectIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/identifiers\n  method: get\n  operationId: getObjectsIdentifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}\n  method: get\n  operationId: getObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}\n  method: patch\n  operationId: patchObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectId}\n  method: delete\n  operationId: deleteObject\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectId}/views\n  method: get\n  operationId: getObjectViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}/attributes\n  method: get\n  operationId: getObjectAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}/attributes/{attributeId}\n  method: get\n  operationId: getObjectAttribute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}/commands\n  method: get\n  operationId: getObjectCommands\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}/commands/{commandId}\n  method: put\n  operationId: putObjectCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectId}/supportedChildTypes\n  method: get\n  operationId: getObjectSupportedChildTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}/points\n  method: get\n  operationId: getObjectPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/batch\n  method: post\n  operationId: postObjectsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectId}/alarms\n  method: get\n  operationId: getObjectAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}/audits\n  method: get\n  operationId: getObjectAudits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/enums/{enumId}\n  method: get\n  operationId: getEnumerationAsJsonSchema\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/objectTypes/{objectType}\n  method: get\n  operationId: getObjectTypeSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeSeries\n  method: get\n  operationId: getTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}/trendedAttributes\n  method: get\n  operationId: getObjectTrendedAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeSeries/{objectId}\n  method: get\n  operationId: getRepoTrendedObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /timeSeries/{objectId}/trendedAttributes\n  method: get\n  operationId: getRepoTrendedAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeSeries/{objectId}/trendedAttributes/{attributeId}\n  method: get\n  operationId: getTrendedAttribute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectId}/trendedAttributes/{attributeId}/samples\n  method: get\n  operationId: getObjectAttributeSamplesFromBuffer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeSeries/{objectId}/trendedAttributes/{attributeId}/samples\n  method: get\n  operationId: getRepoSamples\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeSeries/batch\n  method: post\n  operationId: postRepoBatchTimeSeries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeSeries/streams/{streamId}/subscriptions\n  method: post\n  operationId: postTimeSeriesStreamSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeSeries/streams/{streamId}/subscriptions/{subscriptionId}\n  method: put\n  operationId: putTimeSeriesStreamSubscription\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeSeries/streams/{streamId}/subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteTimeSeriesStreamSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stream\n  method: get\n  operationId: getStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networkDevices\n  method: get\n  operationId: getNetworkDevices\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networkDevices/{networkDeviceId}\n  method: get\n  operationId: getNetworkDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networkDevices/{networkDeviceId}\n  method: delete\n  operationId: deleteNetworkDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networkDevices/{networkDeviceId}/networkDevices\n  method: get\n  operationId: getChildNetworkDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networkDevices/{networkDeviceId}/spaces\n\
  \  method: get\n  operationId: getDeviceSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networkDevices/{networkDeviceId}/equipment\n  method: get\n  operationId: getEquipmentHostedByDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networkDevices/{networkDeviceId}/alarms\n  method: get\n  operationId: getNetworkDeviceAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment\n  method: get\n  operationId: getEquipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/{equipmentId}\n  method: get\n  operationId: getEquipmentInstance\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/{equipmentId}/spaces\n  method: get\n  operationId: getEquipmentSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/{equipmentId}/equipment\n  method: get\n  operationId: getServedByEquipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/{equipmentId}/upstreamEquipment\n  method: get\n  operationId: getUpstreamEquipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/{equipmentId}/networkDevices\n  method: get\n  operationId: getNetworkDevicesHostingEquipment\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/{equipmentId}/points\n  method: get\n  operationId: getEquipmentPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/tree\n  method: get\n  operationId: getEquipmentTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/tree/{objectId}\n  method: get\n  operationId: getEquipmentSubtree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /equipment/{equipmentId}/servedEquipment\n  method: get\n  operationId: getServedEquipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /spaces\n  method: get\n  operationId: getSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}\n  method: get\n  operationId: getSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/spaces\n  method: get\n  operationId: getChildSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/equipment\n  method: get\n  operationId: getEquipmentServingSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/networkDevices\n  method: get\n  operationId: getNetworkDevicesServingSpace\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}/servingEquipment\n  method: get\n  operationId: getSpaceServingEquipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/tree\n  method: get\n  operationId: getSpacesTreeRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/tree/{spaceId}\n  method: get\n  operationId: getSpaceTreeChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alarms/{alarmId}\n  method: get\n  operationId: getAlarm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /alarms/{alarmId}\n  method: patch\n  operationId: patchAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alarms/{alarmId}/annotations\n  method: get\n  operationId: getAlarmAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audits/{auditId}\n  method: get\n  operationId: getAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audits/{auditId}\n  method: patch\n  operationId: patchAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audits/{auditId}/annotations\n  method: get\n  operationId: getAuditAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audits/{auditId}/annotations\n  method: post\n  operationId: postAuditAnnotation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audits/users\n  method: get\n  operationId: getAuditsUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/agentic-access/johnson-controls-agentic-access.yml
summary_line: 70 operations · 16 acting
tags:
- Building Automation
- Energy Storage
- Fire & Security
- HVAC
- Smart Buildings
- Fortune 100
---
