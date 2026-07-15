---
acting_count: 1570
action_class_counts:
  acting: 1570
api_specs:
- filename: bitrix24-openapi.json
  format: json
  label: Bitrix24 REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrix24/refs/heads/main/openapi/bitrix24-openapi.json
consequence_counts:
  physical: 321
  safety-critical: 37
  write: 1212
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 37
kind: agentic-access
layout: agentic-access
method: generated
name: Bitrix24 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bizproc.workflow.kill
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bizproc.workflow.terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.company.details.configuration.reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.contact.details.configuration.reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.deal.details.configuration.reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.documentgenerator.document.enablepublicurl
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.item.details.configuration.reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.lead.details.configuration.reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.add
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.countries
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.field.add
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.field.availabletoadd
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.field.delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.field.fields
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.field.get
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.field.list
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.field.update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.fields
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.get
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.list
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm.requisite.preset.update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /documentgenerator.document.enablepublicurl
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /im.chat.mute
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /im.user.status.idle.end
operation_count: 1570
overview: 'Bitrix24 exposes 1570 API operations that an AI agent could call, of which 1570 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1212 write, 321 physical, and 37 safety-critical.


  37 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bitrix24
provider_slug: bitrix24
slug: bitrix24-agentic-access
source_filename: bitrix24-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bitrix24-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1570\n  by_action_class:\n    acting: 1570\n  by_consequence:\n    write: 1212\n    physical: 321\n    safety-critical: 37\n  human_in_the_loop_required: 37\noperations:\n- path: /BX24.placement.bindEvent\n  method: post\n  operationId: BX24_placement_bindEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - placement\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BX24.placement.call\n  method: post\n  operationId:\
  \ BX24_placement_call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - placement\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BX24.placement.getInterface\n  method: post\n  operationId: BX24_placement_getInterface\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - placement\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BX24.placement.info\n  method: post\n  operationId: BX24_placement_info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - placement\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.MEASURE.ON.ADD\n  method: post\n  operationId: CATALOG_MEASURE_ON_ADD\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.MEASURE.ON.DELETE\n  method: post\n  operationId: CATALOG_MEASURE_ON_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /CATALOG.MEASURE.ON.UPDATE\n  method: post\n  operationId: CATALOG_MEASURE_ON_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.PRICE.ON.ADD\n  method: post\n  operationId: CATALOG_PRICE_ON_ADD\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.PRICE.ON.DELETE\n  method: post\n  operationId: CATALOG_PRICE_ON_DELETE\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.PRICE.ON.UPDATE\n  method: post\n  operationId: CATALOG_PRICE_ON_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.PRICE.TYPE.ON.ADD\n  method: post\n  operationId: CATALOG_PRICE_TYPE_ON_ADD\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.PRICE.TYPE.ON.DELETE\n  method: post\n  operationId: CATALOG_PRICE_TYPE_ON_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.PRICE.TYPE.ON.UPDATE\n  method: post\n  operationId: CATALOG_PRICE_TYPE_ON_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n \
  \     exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.PRODUCT.ON.ADD\n  method: post\n  operationId: CATALOG_PRODUCT_ON_ADD\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.PRODUCT.ON.DELETE\n  method: post\n  operationId: CATALOG_PRODUCT_ON_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.PRODUCT.ON.UPDATE\n  method: post\n  operationId: CATALOG_PRODUCT_ON_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.ROUNDING.ON.ADD\n  method: post\n  operationId: CATALOG_ROUNDING_ON_ADD\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.ROUNDING.ON.DELETE\n\
  \  method: post\n  operationId: CATALOG_ROUNDING_ON_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CATALOG.ROUNDING.ON.UPDATE\n  method: post\n  operationId: CATALOG_ROUNDING_ON_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - catalog\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access.name\n  method: post\n  operationId: access_name\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - basic\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai.engine.list\n  method: post\n  operationId: ai_engine_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ai_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai.engine.register\n  method: post\n  operationId: ai_engine_register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ai_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /ai.engine.unregister\n  method: post\n  operationId: ai_engine_unregister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ai_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app.info\n  method: post\n  operationId: app_info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app.option.get\n  method: post\n  operationId: app_option_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app.option.set\n  method: post\n  operationId: app_option_set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.connector.add\n  method: post\n  operationId: biconnector_connector_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.connector.delete\n  method: post\n  operationId: biconnector_connector_delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.connector.fields\n  method: post\n  operationId: biconnector_connector_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.connector.get\n  method: post\n  operationId: biconnector_connector_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.connector.list\n  method: post\n  operationId: biconnector_connector_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.connector.update\n  method: post\n  operationId: biconnector_connector_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.dataset.add\n  method: post\n  operationId: biconnector_dataset_add\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.dataset.delete\n  method: post\n  operationId: biconnector_dataset_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.dataset.fields\n  method: post\n  operationId: biconnector_dataset_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.dataset.fields.update\n  method: post\n  operationId: biconnector_dataset_fields_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.dataset.get\n  method: post\n  operationId: biconnector_dataset_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.dataset.list\n  method: post\n  operationId: biconnector_dataset_list\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.dataset.update\n  method: post\n  operationId: biconnector_dataset_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.source.add\n  method: post\n  operationId: biconnector_source_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.source.delete\n  method: post\n  operationId: biconnector_source_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.source.fields\n  method: post\n  operationId: biconnector_source_fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.source.get\n  method: post\n  operationId: biconnector_source_get\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.source.list\n  method: post\n  operationId: biconnector_source_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biconnector.source.update\n  method: post\n  operationId: biconnector_source_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - biconnector\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.activity.add\n  method: post\n  operationId: bizproc_activity_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.activity.delete\n  method: post\n  operationId: bizproc_activity_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.activity.list\n  method: post\n  operationId: bizproc_activity_list\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.activity.log\n  method: post\n  operationId: bizproc_activity_log\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.activity.update\n  method: post\n  operationId: bizproc_activity_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.event.send\n  method: post\n  operationId: bizproc_event_send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.robot.add\n  method: post\n  operationId: bizproc_robot_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.robot.delete\n  method: post\n  operationId: bizproc_robot_delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.robot.list\n  method: post\n  operationId: bizproc_robot_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.robot.update\n  method: post\n  operationId: bizproc_robot_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /bizproc.task.complete\n  method: post\n  operationId: bizproc_task_complete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.task.delegate\n  method: post\n  operationId: bizproc_task_delegate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.task.list\n  method: post\n  operationId: bizproc_task_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.workflow.instances\n  method: post\n  operationId: bizproc_workflow_instances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.workflow.kill\n  method: post\n  operationId: bizproc_workflow_kill\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /bizproc.workflow.start\n  method: post\n  operationId: bizproc_workflow_start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.workflow.template.add\n  method: post\n  operationId: bizproc_workflow_template_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.workflow.template.delete\n  method: post\n  operationId: bizproc_workflow_template_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.workflow.template.list\n  method: post\n  operationId: bizproc_workflow_template_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.workflow.template.update\n  method: post\n  operationId: bizproc_workflow_template_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /bizproc.workflow.terminate\n  method: post\n  operationId: bizproc_workflow_terminate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - bizproc\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /booking.v1.booking.add\n  method: post\n  operationId: booking_v1_booking_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.client.list\n  method: post\n  operationId: booking_v1_booking_client_list\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.client.set\n  method: post\n  operationId: booking_v1_booking_client_set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.client.unset\n  method: post\n  operationId: booking_v1_booking_client_unset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.createfromwaitlist\n  method: post\n  operationId: booking_v1_booking_createfromwaitlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.delete\n  method: post\n  operationId: booking_v1_booking_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.externalData.list\n  method: post\n  operationId: booking_v1_booking_externalData_list\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.externalData.set\n  method: post\n  operationId: booking_v1_booking_externalData_set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.externalData.unset\n  method: post\n  operationId: booking_v1_booking_externalData_unset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.get\n  method: post\n  operationId: booking_v1_booking_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.list\n  method: post\n  operationId: booking_v1_booking_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.booking.update\n  method: post\n  operationId:\
  \ booking_v1_booking_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.clienttype.list\n  method: post\n  operationId: booking_v1_clienttype_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.resource.add\n  method: post\n  operationId: booking_v1_resource_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.resource.delete\n  method: post\n  operationId: booking_v1_resource_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.resource.get\n  method: post\n  operationId: booking_v1_resource_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking.v1.resource.list\n  method: post\n  operationId: booking_v1_resource_list\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - booking\n    audience: null\n    token:\n      max-ttl: 900\n  \n\n# --- truncated at 32 KB (594 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/bitrix24/refs/heads/main/agentic-access/bitrix24-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitrix24/refs/heads/main/agentic-access/bitrix24-agentic-access.yml
summary_line: 1570 operations · 1570 acting · 37 human-in-the-loop
tags:
- CRM
- Collaboration
- Project Management
- Tasks
- Telephony
- Contact Center
- Document Management
- HR
- Business Suite
---
