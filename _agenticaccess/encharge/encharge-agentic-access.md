---
acting_count: 43
action_class_counts:
  acting: 43
  connected: 26
api_specs:
- filename: TVRj5o3E
  format: yaml
  label: Encharge Transactional Email API
  slug: transactional-email-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/460427/TVRj5o3E
- filename: SVfNwVFU
  format: yaml
  label: Encharge Ingest API
  slug: ingest-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/460427/SVfNwVFU
- filename: encharge-account-api-openapi.yml
  format: yaml
  label: Encharge Account API
  slug: encharge-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-account-api-openapi.yml
- filename: encharge-broadcasts-api-openapi.yml
  format: yaml
  label: Encharge Broadcasts API
  slug: encharge-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-broadcasts-api-openapi.yml
- filename: encharge-customobjects-api-openapi.yml
  format: yaml
  label: Encharge Custom Objects API
  slug: encharge-customobjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-customobjects-api-openapi.yml
- filename: encharge-customobjectsschema-api-openapi.yml
  format: yaml
  label: Encharge Custom Objects Schema API
  slug: encharge-customobjectsschema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-customobjectsschema-api-openapi.yml
- filename: encharge-emailtemplates-api-openapi.yml
  format: yaml
  label: Encharge Email Templates API
  slug: encharge-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-emailtemplates-api-openapi.yml
- filename: encharge-folders-api-openapi.yml
  format: yaml
  label: Encharge Folders API
  slug: encharge-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-folders-api-openapi.yml
- filename: encharge-people-api-openapi.yml
  format: yaml
  label: Encharge People API
  slug: encharge-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-people-api-openapi.yml
- filename: encharge-personfields-api-openapi.yml
  format: yaml
  label: Encharge Person Fields API
  slug: encharge-personfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-personfields-api-openapi.yml
- filename: encharge-segments-api-openapi.yml
  format: yaml
  label: Encharge Segments API
  slug: encharge-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-segments-api-openapi.yml
- filename: encharge-settings-api-openapi.yml
  format: yaml
  label: Encharge Email Domain Settings API
  slug: encharge-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-settings-api-openapi.yml
- filename: encharge-tags-api-openapi.yml
  format: yaml
  label: Encharge Tags API
  slug: encharge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-tags-api-openapi.yml
- filename: encharge-tags-management-api-openapi.yml
  format: yaml
  label: Encharge Tags Management API
  slug: encharge-tags-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-tags-management-api-openapi.yml
- filename: encharge-webhooks-api-openapi.yml
  format: yaml
  label: Encharge Webhooks API
  slug: encharge-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 26
  write: 42
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Encharge Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /broadcasts/{id}/send
operation_count: 69
overview: 'Encharge exposes 69 API operations that an AI agent could call, of which 43 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 42 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Encharge
provider_slug: encharge
slug: encharge-agentic-access
source_filename: encharge-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/encharge-account-api-openapi.yml, openapi/encharge-broadcasts-api-openapi.yml,\n  openapi/encharge-customobjects-api-openapi.yml, openapi/encharge-customobjectsschema-api-openapi.yml,\n  openapi/encharge-emailtemplates-api-openapi.yml, openapi/encharge-folders-api-openapi.yml,\n  openapi/encharge-people-api-openapi.yml, openapi/encharge-personfields-api-openapi.yml, openapi/encharge-segments-api-openapi.yml,\n  openapi/encharge-settings-api-openapi.yml, openapi/encharge-tags-api-openapi.yml, openapi/encharge-tags-management-api-openapi.yml,\n  openapi/encharge-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    connected: 26\n    acting:\
  \ 43\n  by_consequence:\n    read: 26\n    physical: 1\n    write: 42\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/info\n  method: get\n  operationId: GetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/form/{formId}\n  method: get\n  operationId: GetAccountInfoByFormId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broadcasts/{id}/send\n  method: post\n  operationId: SendBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - broadcasts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /objects/{objectName}\n  method: get\n  operationId: GetCustomObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectName}\n  method: post\n  operationId: CreateCustomObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectName}\n  method: put\n  operationId: CreateOrUpdateCustomObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectName}/segments/{segmentId}\n\
  \  method: get\n  operationId: GetCustomObjectsInSegment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectName}/count\n  method: get\n  operationId: GetCustomObjectsCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectName}/segments/{segmentId}/count\n  method: get\n  operationId: GetCustomObjectsInSegmentCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectName}/search\n  method: get\n  operationId: SearchCustomObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectName}/{id}\n  method: get\n  operationId:\
  \ GetCustomObjectById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectName}/{id}\n  method: patch\n  operationId: UpdateCustomObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectName}/{id}\n  method: delete\n  operationId: DeleteCustomObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectName}/externalId/{externalId}\n\
  \  method: get\n  operationId: GetCustomObjectByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectName}/externalId/{externalId}\n  method: patch\n  operationId: UpdateCustomObjectByExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectName}/externalId/{externalId}\n  method: delete\n  operationId: DeleteCustomObjectByExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectName}/{id}/associations/{associationId}\n  method: get\n  operationId: GetObjectsByAssociation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectName}/{id}/associations\n  method: get\n  operationId: GetAllAssociatedObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{objectName}/{id}/associations/default/{targetObjectName}/{targetId}\n  method: post\n  operationId: AssociateObjectsByDefaultAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectName}/{id}/associations/{associationId}/{targetId}\n  method: post\n  operationId: AssociateCustomObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{objectName}/{id}/associations/{associationId}/{targetId}\n  method: delete\n  operationId: RemoveCustomObjectsAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /schemas\n  method: get\n  operationId: GetCustomObjectsSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas\n  method: post\n  operationId: CreateCustomObjectSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas/{objectName}\n  method: get\n  operationId: GetCustomObjectSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/{objectName}\n  method: patch\n  operationId: UpdateCustomObjectSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    -\
  \ account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas/{objectName}\n  method: delete\n  operationId: DeleteCustomObjectSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas/{objectName}/fields\n  method: post\n  operationId: CreateObjectFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - personFields:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /schemas/{objectName}/fields/{fieldName}\n  method: patch\n  operationId: EditObjectField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - personFields:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas/{objectName}/fields/{fieldName}\n  method: delete\n  operationId: DeleteObjectField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - personFields:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas/associations\n  method: post\n  operationId: DefineCustomObjectsAssociationSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas/associations/{id}\n  method: delete\n  operationId: RemoveCustomObjectsAssociationSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/{id}\n  method: get\n  operationId: GetEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - emails:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/{id}\n  method: patch\n  operationId: ModifyEmail\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - emails:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/{id}\n  method: delete\n  operationId: DeleteEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - emails:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails\n  method: post\n  operationId: CreateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - emails:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /emails/{id}/versions\n  method: get\n  operationId: GetEmailVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - emails:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/{id}/versions/{version}\n  method: get\n  operationId: GetEmailVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - emails:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/{id}/versions/selected\n  method: get\n  operationId: GetSelectedEmailVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - emails:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/{id}/versions/latest\n  method: patch\n  operationId: UpdateLatestEmailVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - emails:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emails/{id}/versions/{version}/restore\n  method: post\n  operationId: RestoreEmailVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - emails:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders\n  method: post\n  operationId: CreateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders/{id}\n  method: patch\n\
  \  operationId: EditFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people\n  method: delete\n  operationId: ArchivePeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - people:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people\n  method: get\n  operationId: GetSpecificPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - people:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people\n  method: post\n  operationId: CreateUpdatePeople\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - people:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/all\n  method: get\n  operationId: GetAllPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - people:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/unsubscribe\n  method: post\n  operationId: UnsubscribePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - people:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields\n  method: get\n  operationId: GetFields\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields\n  method: post\n  operationId: CreateFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - personFields:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields/{fieldName}\n  method: patch\n  operationId: EditField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - personFields:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields/{fieldName}\n  method: delete\n  operationId: DeleteField\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - personFields:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /segments\n  method: get\n  operationId: GetSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - people:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /segments\n  method: post\n  operationId: CreateSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - people:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /segments/{segmentId}/people\n  method: get\n  operationId: GetPeopleInSegment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - people:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /segments/{id}\n  method: patch\n  operationId: ModifySegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - people:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/email/domains\n  method: get\n  operationId: GetDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/email/domains\n  method: post\n  operationId: CreateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - emailSettings:write\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/email/domains/{id}\n  method: get\n  operationId: GetDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/email/domains/{id}\n  method: delete\n  operationId: DeleteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - emailSettings:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/email/domains/{id}/verify\n  method: post\n  operationId: VerifyDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - emailSettings:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags\n  method: post\n  operationId: AddTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - people:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags\n  method: delete\n  operationId: RemoveTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - people:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags-management\n  method: get\n  operationId: GetAccountTags\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags-management\n  method: post\n  operationId: CreateAccountTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags-management/counts\n  method: get\n  operationId: GetTagCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags-management/{tag}\n  method: patch\n  operationId: UpdateAccountTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags-management/{tag}\n  method: delete\n  operationId: DeleteAccountTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event-subscriptions\n  method: post\n  operationId: CreateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event-subscriptions/{id}\n  method: delete\n  operationId: DeleteWebhook\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - account:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/agentic-access/encharge-agentic-access.yml
summary_line: 69 operations · 43 acting
tags:
- Email Marketing
- Marketing Automation
- Transactional Email
- Software-as-a-Service
- Behavioral Email
- Customer Engagement
- Customer Data
- Webhook
---
