---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 17
api_specs:
- filename: flock-safety-alerts-api-openapi.yml
  format: yaml
  label: Flock Safety Alerts API
  slug: flock-safety-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-alerts-api-openapi.yml
- filename: flock-safety-cad-events-api-openapi.yml
  format: yaml
  label: Flock Safety CAD Events API
  slug: flock-safety-cad-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-cad-events-api-openapi.yml
- filename: flock-safety-custom-hotlists-api-openapi.yml
  format: yaml
  label: Flock Safety Custom Hotlists API
  slug: flock-safety-custom-hotlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-custom-hotlists-api-openapi.yml
- filename: flock-safety-devices-api-openapi.yml
  format: yaml
  label: Flock Safety Devices API
  slug: flock-safety-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-devices-api-openapi.yml
- filename: flock-safety-lpr-hotlist-alert-subscriptions-api-openapi.yml
  format: yaml
  label: Flock Safety LPR Hotlist Alert Subscriptions API
  slug: flock-safety-lpr-hotlist-alert-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-lpr-hotlist-alert-subscriptions-api-openapi.yml
- filename: flock-safety-plate-reads-api-openapi.yml
  format: yaml
  label: Flock Safety Plate Reads API
  slug: flock-safety-plate-reads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-plate-reads-api-openapi.yml
- filename: flock-safety-tracked-subject-types-api-openapi.yml
  format: yaml
  label: Flock Safety Tracked Subject Types API
  slug: flock-safety-tracked-subject-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-tracked-subject-types-api-openapi.yml
- filename: flock-safety-tracked-subjects-api-openapi.yml
  format: yaml
  label: Flock Safety Tracked Subjects API
  slug: flock-safety-tracked-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-tracked-subjects-api-openapi.yml
- filename: flock-safety-vehicle-images-api-openapi.yml
  format: yaml
  label: Flock Safety Vehicle Images API
  slug: flock-safety-vehicle-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-vehicle-images-api-openapi.yml
- filename: flock-safety-oauth2-api-openapi.yml
  format: yaml
  label: Flock Safety O Auth2 API
  slug: flock-safety-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-oauth2-api-openapi.yml
consequence_counts:
  read: 17
  safety-critical: 1
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Flock Safety Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /geo/subjects/{externalSubjectId}
operation_count: 43
overview: 'Flock Safety exposes 43 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 25 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flock Safety
provider_slug: flock-safety
slug: flock-safety-agentic-access
source_filename: flock-safety-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/flock-safety-alerts-api-openapi.yml, openapi/flock-safety-cad-events-api-openapi.yml,\n  openapi/flock-safety-custom-hotlists-api-openapi.yml, openapi/flock-safety-devices-api-openapi.yml,\n  openapi/flock-safety-lpr-hotlist-alert-subscriptions-api-openapi.yml, openapi/flock-safety-oauth2-api-openapi.yml,\n  openapi/flock-safety-plate-reads-api-openapi.yml, openapi/flock-safety-tracked-subject-types-api-openapi.yml,\n  openapi/flock-safety-tracked-subjects-api-openapi.yml, openapi/flock-safety-vehicle-images-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 17\n    acting: 26\n  by_consequence:\n    read: 17\n    write: 25\n    safety-critical:\
  \ 1\n  human_in_the_loop_required: 1\noperations:\n- path: /alerts/{alertId}\n  method: get\n  operationId: getAlertsByAlertId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts/{alertId}\n  method: put\n  operationId: putAlertsByAlertId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts\n  method: get\n  operationId: getAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts\n  method: post\n  operationId: postAlerts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/{alertId}/close\n  method: post\n  operationId: postAlertsByAlertIdClose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cad/events/active\n  method: get\n  operationId: getCadEventsActive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cad/events/active\n  method: post\n  operationId: postCadEventsActive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cad/events/{externalId}\n  method: get\n  operationId: getCadEventsByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cad/events\n  method: get\n  operationId: getCadEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cad/events\n  method: post\n  operationId: postCadEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cad/events/{externalId}/close\n  method: post\n  operationId: postCadEventsByExternalIdClose\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cad/events/{externalId}/narrative\n  method: post\n  operationId: postCadEventsByExternalIdNarrative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cad/events/{externalId}/open\n  method: post\n  operationId: postCadEventsByExternalIdOpen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /cad/events/externalIds\n  method: post\n  operationId: postCadEventsExternalIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotlists/{hotlistId}\n  method: delete\n  operationId: deleteHotlistsByHotlistId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom-hotlists:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotlists/{hotlistId}\n  method: get\n  operationId: getHotlistsByHotlistId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - custom-hotlists:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotlists/{hotlistId}\n  method: put\n  operationId: putHotlistsByHotlistId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom-hotlists:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotlists/{hotlistId}/entries\n  method: get\n  operationId: getHotlistsByHotlistIdEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - custom-hotlists:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotlists\n  method: get\n  operationId: getHotlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - custom-hotlists:read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /hotlists\n  method: post\n  operationId: postHotlists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom-hotlists:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotlists/{hotlistId}/entries/addBatch\n  method: post\n  operationId: postHotlistsByHotlistIdEntriesAddBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - custom-hotlists:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotlists/{hotlistId}/entries/deleteBatch\n  method: post\n  operationId: postHotlistsByHotlistIdEntriesDeleteBatch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - custom-hotlists:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}\n  method: get\n  operationId: getDevicesByDeviceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceId}\n  method: patch\n  operationId: patchDevicesByDeviceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices\n  method: get\n  operationId: getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: post\n  operationId: postDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}/decommission\n  method: post\n  operationId: postDevicesByDeviceIdDecommission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/lpr/alerts/subscriptions/{id}\n  method: delete\n  operationId: deleteIntegrationsLprAlertsSubscriptionsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/lpr/alerts/subscriptions/{id}\n  method: get\n  operationId: getIntegrationsLprAlertsSubscriptionsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/lpr/alerts/subscriptions\n  method: get\n  operationId: getIntegrationsLprAlertsSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/lpr/alerts/subscriptions\n  method: post\n  operationId: postIntegrationsLprAlertsSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/lpr/alerts/subscriptions\n  method: put\n  operationId: putIntegrationsLprAlertsSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: postOauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reads/lookup/page/{pageId}\n  method: get\n  operationId: getReadsLookupPageByPageId\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reads/lookup\n  method: post\n  operationId: postReadsLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geo/types/{typeId}\n  method: delete\n  operationId: deleteGeoTypesByTypeId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geo/types\n  method: get\n  operationId: getGeoTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geo/types\n  method: post\n  operationId: postGeoTypes\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geo/subjects/{externalSubjectId}\n  method: delete\n  operationId: deleteGeoSubjectsByExternalSubjectId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /geo/subjects/{externalSubjectId}\n  method: get\n  operationId: getGeoSubjectsByExternalSubjectId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geo/subjects\n  method: get\n  operationId: getGeoSubjects\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geo/subjects\n  method: put\n  operationId: putGeoSubjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}/images\n  method: post\n  operationId: postDevicesByDeviceIdImages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/agentic-access/flock-safety-agentic-access.yml
summary_line: 43 operations · 26 acting · 1 human-in-the-loop
tags:
- Company
- American Dynamism
- Public Safety
- Law Enforcement
- License Plate Recognition
- LPR
- Physical Security
- Surveillance
- Computer Vision
- Webhook
- Geolocation
- CAD
---
