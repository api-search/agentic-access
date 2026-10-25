---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 62
api_specs:
- filename: openspace-custom-field-notes-api-openapi.yml
  format: yaml
  label: OpenSpace Custom Field Notes API
  slug: openspace-custom-field-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-custom-field-notes-api-openapi.yml
- filename: openspace-external-executive-view-controller-api-openapi.yml
  format: yaml
  label: OpenSpace External Executive View Controller API
  slug: openspace-external-executive-view-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-external-executive-view-controller-api-openapi.yml
- filename: openspace-field-notes-api-openapi.yml
  format: yaml
  label: OpenSpace Field notes API
  slug: openspace-field-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-field-notes-api-openapi.yml
- filename: openspace-global-config-api-openapi.yml
  format: yaml
  label: OpenSpace Global config API
  slug: openspace-global-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-global-config-api-openapi.yml
- filename: openspace-images-api-openapi.yml
  format: yaml
  label: OpenSpace Images API
  slug: openspace-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-images-api-openapi.yml
- filename: openspace-organizations-api-openapi.yml
  format: yaml
  label: OpenSpace Organizations API
  slug: openspace-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-organizations-api-openapi.yml
- filename: openspace-progress-tracking-api-openapi.yml
  format: yaml
  label: OpenSpace Progress Tracking API
  slug: openspace-progress-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-progress-tracking-api-openapi.yml
- filename: openspace-reports-api-openapi.yml
  format: yaml
  label: OpenSpace Reports API
  slug: openspace-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-reports-api-openapi.yml
- filename: openspace-sites-api-openapi.yml
  format: yaml
  label: OpenSpace Sites API
  slug: openspace-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-sites-api-openapi.yml
- filename: openspace-webhook-deliveries-api-openapi.yml
  format: yaml
  label: OpenSpace Webhook Deliveries API
  slug: openspace-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-webhook-deliveries-api-openapi.yml
- filename: openspace-webhook-headers-api-openapi.yml
  format: yaml
  label: OpenSpace Webhook Headers API
  slug: openspace-webhook-headers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-webhook-headers-api-openapi.yml
- filename: openspace-webhook-rules-api-openapi.yml
  format: yaml
  label: OpenSpace Webhook Rules API
  slug: openspace-webhook-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-webhook-rules-api-openapi.yml
- filename: openspace-webhooks-api-openapi.yml
  format: yaml
  label: OpenSpace Webhooks API
  slug: openspace-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/openapi/openspace-webhooks-api-openapi.yml
consequence_counts:
  read: 62
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openspace Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 76
overview: 'OpenSpace exposes 76 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 62 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenSpace
provider_slug: openspace
slug: openspace-agentic-access
source_filename: openspace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/openspace-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 76\n  by_action_class:\n    connected: 62\n    acting: 14\n  by_consequence:\n    read: 62\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /api/external/v1/global-config\n  method: get\n  operationId: getGlobalConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations\n  method: get\n  operationId: organizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/external/v1/organizations/{organizationId}\n  method: get\n  operationId: organizationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/sites\n  method: get\n  operationId: sitesByOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/deliveries\n  method: get\n  operationId: listDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/deliveries/{deliveryId}\n  method: get\n  operationId: getDeliveryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/deliveries/{deliveryId}/redeliver\n  method: post\n  operationId: redeliverEvent\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/headers\n  method: get\n  operationId: listHeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/headers\n  method: post\n  operationId: createHeader\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/headers/{headerId}\n\
  \  method: delete\n  operationId: deleteHeader\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/headers/{headerId}\n  method: get\n  operationId: getHeader\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/headers/{headerId}\n  method: patch\n  operationId: updateHeader\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/rules\n  method: get\n  operationId: listRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/rules\n  method: post\n  operationId: createRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/rules/{ruleId}\n  method: delete\n  operationId: deleteRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/rules/{ruleId}\n  method: get\n  operationId: getRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/rules/{ruleId}\n  method: patch\n  operationId: updateRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/update-secret\n  method: post\n  operationId: updateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/organizations/{organizationId}/webhooks/{webhookId}/verify\n  method: post\n  operationId: verifyWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /api/external/v1/reports/360-videos\n  method: get\n  operationId: getReporting360Videos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/reports/drone-images\n  method: get\n  operationId: getReportingDroneImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/reports/field-notes\n  method: get\n  operationId: getReportingFieldNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/reports/memberships\n  method: get\n  operationId: getMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /api/external/v1/reports/organizations\n  method: get\n  operationId: getReportingOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/reports/sheets\n  method: get\n  operationId: getReportingSheets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/reports/site-events\n  method: get\n  operationId: getReportingSiteEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/reports/sites\n  method: get\n  operationId: getReportingSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}\n\
  \  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/captures\n  method: get\n  operationId: capturesBySite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/captures/{captureId}\n  method: get\n  operationId: capturesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/captures/{captureId}/panos\n  method: get\n  operationId: getPanos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/captures/{captureId}/panos/{panoId}/equi\n\
  \  method: get\n  operationId: downloadOrReprojectEquirectangularImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/captures/{captureId}/panos/{panoId}/image\n  method: get\n  operationId: getImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/captures/{captureId}/panos/{panoId}/preview-equi\n  method: get\n  operationId: previewEquirectangularImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/custom-field-notes/search\n  method: post\n  operationId: searchCustomFieldNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/custom-field-notes/{customFieldNoteId}/attachments/{attachmentId}/download\n  method: get\n  operationId: downloadAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/custom-field-notes/{customFieldNoteId}/comments\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/custom-field-notes/{customFieldNoteId}/photos/{photoId}/image\n  method: get\n  operationId: getPhotoImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/field-note-statuses\n  method:\
  \ get\n  operationId: getFieldNoteStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/field-notes\n  method: get\n  operationId: fieldNotesBySite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/field-notes/search\n  method: post\n  operationId: searchFieldNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/field-notes/{fieldNoteId}\n  method: get\n  operationId: fieldNoteById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/field-notes/{fieldNoteId}/activity-log\n\
  \  method: get\n  operationId: activityLogByFieldNoteId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/field-notes/{fieldNoteId}/attachment/{attachmentId}/download\n  method: get\n  operationId: downloadFieldNoteAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/field-notes/{fieldNoteId}/comments\n  method: get\n  operationId: commentsByFieldNoteId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/field-notes/{fieldNoteId}/comments\n  method: post\n  operationId: addComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external/v1/sites/{siteId}/field-notes/{fieldNoteId}/image\n  method: get\n  operationId: downloadFieldNoteImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/executive-view/batches\n  method: get\n  operationId: getExecutiveViewBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/executive-view/chart-progresses/search\n  method: post\n  operationId: searchExecutiveViewChartProgresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/executive-view/subcontractors/search\n  method: post\n  operationId: searchExecutiveViewSubcontractors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/executive-view/tasks/search\n  method: post\n  operationId: searchExecutiveViewTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/executive-view/tree\n  method: get\n  operationId: getExecutiveViewTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/floorplans\n  method:\
  \ get\n  operationId: getFloorplans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/floorplans/{floorplanId}/image\n  method: get\n  operationId: getFloorplanImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/phases\n  method: get\n  operationId: getPhases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/progress-dates\n  method: get\n  operationId: getProgressDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/spaces\n\
  \  method: get\n  operationId: getSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/spaces/{spaceId}/progress/components\n  method: get\n  operationId: getComponentProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/spaces/{spaceId}/progress/subcontractors\n  method: get\n  operationId: getSubcontractorProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/spaces/{spaceId}/progress/tasks\n  method: get\n  operationId: getTaskProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/spaces/{spaceId}/scenes\n  method: get\n  operationId: getScenes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/spaces/{spaceId}/scenes/{sceneId}/shots\n  method: get\n  operationId: getShots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/spaces/{spaceId}/scenes/{sceneId}/shots/{shotId}/image\n  method: get\n  operationId: getShotImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/spaces/{spaceId}/scenes/{sceneId}/spotlights\n\
  \  method: get\n  operationId: getSpotlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/progress-tracking/spaces/{spaceId}/scenes/{sceneId}/spotlights/{spotlightId}\n  method: get\n  operationId: getSpotlight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/sheet/{sheetId}/image\n  method: get\n  operationId: getSheetImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/sheets\n  method: get\n  operationId: sheetsBySite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/external/v1/sites/{siteId}/sheets/{sheetId}\n  method: get\n  operationId: sheetsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/sheets/{sheetId}/captures\n  method: get\n  operationId: captures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external/v1/sites/{siteId}/zones\n  method: get\n  operationId: getZonesBySite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openspace/refs/heads/main/agentic-access/openspace-agentic-access.yml
summary_line: 76 operations · 14 acting
tags:
- Construction Technology
- Visual Intelligence
- 360 Camera
- Jobsite Documentation
- Progress Tracking
- BIM
- Drone Imagery
- Computer Vision
- Artificial Intelligence
- Software-as-a-Service
- San Francisco
---
