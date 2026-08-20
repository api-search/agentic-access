---
acting_count: 61
action_class_counts:
  acting: 61
  connected: 1
api_specs:
- filename: withings-answers-api-openapi.yml
  format: yaml
  label: Withings answers API
  slug: withings-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-answers-api-openapi.yml
- filename: withings-device-api-openapi.yml
  format: yaml
  label: Withings device API
  slug: withings-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-device-api-openapi.yml
- filename: withings-dropshipment-api-openapi.yml
  format: yaml
  label: Withings dropshipment API
  slug: withings-dropshipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-dropshipment-api-openapi.yml
- filename: withings-heart-api-openapi.yml
  format: yaml
  label: Withings heart API
  slug: withings-heart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-heart-api-openapi.yml
- filename: withings-measure-api-openapi.yml
  format: yaml
  label: Withings measure API
  slug: withings-measure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-measure-api-openapi.yml
- filename: withings-notify-api-openapi.yml
  format: yaml
  label: Withings notify API
  slug: withings-notify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-notify-api-openapi.yml
- filename: withings-nudge-api-openapi.yml
  format: yaml
  label: Withings nudge API
  slug: withings-nudge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-nudge-api-openapi.yml
- filename: withings-nudgecampaign-api-openapi.yml
  format: yaml
  label: Withings nudgecampaign API
  slug: withings-nudgecampaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-nudgecampaign-api-openapi.yml
- filename: withings-oauth2-api-openapi.yml
  format: yaml
  label: Withings oauth2 API
  slug: withings-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-oauth2-api-openapi.yml
- filename: withings-order-api-openapi.yml
  format: yaml
  label: Withings order API
  slug: withings-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-order-api-openapi.yml
- filename: withings-rawdata-api-openapi.yml
  format: yaml
  label: Withings rawdata API
  slug: withings-rawdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-rawdata-api-openapi.yml
- filename: withings-signature-api-openapi.yml
  format: yaml
  label: Withings signature API
  slug: withings-signature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-signature-api-openapi.yml
- filename: withings-sleep-api-openapi.yml
  format: yaml
  label: Withings sleep API
  slug: withings-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-sleep-api-openapi.yml
- filename: withings-stetho-api-openapi.yml
  format: yaml
  label: Withings stetho API
  slug: withings-stetho-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-stetho-api-openapi.yml
- filename: withings-survey-api-openapi.yml
  format: yaml
  label: Withings survey API
  slug: withings-survey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-survey-api-openapi.yml
- filename: withings-user-api-openapi.yml
  format: yaml
  label: Withings user API
  slug: withings-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/openapi/withings-user-api-openapi.yml
consequence_counts:
  physical: 6
  read: 1
  safety-critical: 3
  write: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Withings Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: '    https://wbsapi.withings.net/v2/oauth2'
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: 'https://wbsapi.withings.net/notify    '
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: 'https://wbsapi.withings.net/v2/device  '
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: https://wbsapi.withings.net/v2/dropshipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: 'https://wbsapi.withings.net/v2/dropshipment '
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: 'https://wbsapi.withings.net/v2/dropshipment  '
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: 'https://wbsapi.withings.net/v2/dropshipment   '
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: 'https://wbsapi.withings.net/v2/dropshipment    '
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: https://wbsapi.withings.net/v2/order
operation_count: 62
overview: 'Withings exposes 62 API operations that an AI agent could call, of which 61 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 52 write, 6 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Withings
provider_slug: withings
slug: withings-agentic-access
source_filename: withings-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/withings-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 62\n  by_action_class:\n    connected: 1\n    acting: 61\n  by_consequence:\n    read: 1\n    write: 52\n    safety-critical: 3\n    physical: 6\n  human_in_the_loop_required: 3\noperations:\n- path: https://account.withings.com/oauth2_user/authorize2\n  method: get\n  operationId: oauth2-authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: https://wbsapi.withings.net/v2/oauth2\n  method: post\n  operationId: oauth2-getaccesstoken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '  https://wbsapi.withings.net/v2/oauth2'\n  method: post\n  operationId: oauth2-recoverauthorizationcode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '   https://wbsapi.withings.net/v2/oauth2'\n  method: post\n  operationId: oauth2-listusers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '    https://wbsapi.withings.net/v2/oauth2'\n\
  \  method: post\n  operationId: oauth2-revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: '     https://wbsapi.withings.net/v2/oauth2'\n  method: post\n  operationId: oauth2-getdemoaccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '      https://wbsapi.withings.net/v2/oauth2'\n  method: post\n  operationId: oauth2-createclient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/measure\n  method: post\n  operationId: measure-getmeas\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/notify '\n  method: post\n  operationId: notify-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/notify  '\n  method: post\n  operationId: notify-list\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/notify    '\n  method: post\n  operationId: notify-revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: https://wbsapi.withings.net/notify\n  method: post\n  operationId: notify-subscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: 'https://wbsapi.withings.net/notify   '\n  method: post\n  operationId: notify-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/answers\n  method: post\n  operationId: answersv2-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/device  '\n  method: post\n  operationId: devicev2-disablefeature\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/device '\n  method: post\n  operationId: devicev2-enablefeature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/device\n  method: post\n  operationId: devicev2-endpartnerprogram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/dropshipment\n  method:\
  \ post\n  operationId: dropshipmentv2-createorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/dropshipment '\n  method: post\n  operationId: dropshipmentv2-createuserorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/dropshipment   '\n  method: post\n  operationId: dropshipmentv2-delete\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/dropshipment  '\n  method: post\n  operationId: dropshipmentv2-getorderstatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/dropshipment    '\n  method: post\n  operationId: dropshipmentv2-update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/heart '\n  method: post\n  operationId: heartv2-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/heart\n  method: post\n  operationId: heartv2-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/measure   '\n  method: post\n  operationId: measurev2-confirmuser\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/measure\n  method: post\n  operationId: measurev2-getactivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/measure  '\n  method: post\n  operationId: measurev2-getintradayactivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/measure '\n  method: post\n  operationId: measurev2-getworkouts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudge  '\n  method: post\n  operationId: nudgev2-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudge    '\n  method: post\n  operationId: nudgev2-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudge '\n  method: post\n  operationId: nudgev2-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/nudge\n  method: post\n  operationId: nudgev2-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudge   '\n  method: post\n  operationId: nudgev2-update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudgecampaign     '\n  method: post\n  operationId: nudgecampaignv2-addusers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudgecampaign  '\n  method: post\n  operationId: nudgecampaignv2-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudgecampaign    '\n  method: post\n  operationId: nudgecampaignv2-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudgecampaign '\n  method: post\n  operationId: nudgecampaignv2-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/nudgecampaign\n  method: post\n  operationId: nudgecampaignv2-list\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudgecampaign       '\n  method: post\n  operationId: nudgecampaignv2-listusers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/nudgecampaign      '\n  method: post\n  operationId: nudgecampaignv2-removeusers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: 'https://wbsapi.withings.net/v2/nudgecampaign   '\n  method: post\n  operationId: nudgecampaignv2-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/order\n  method: post\n  operationId: orderv2-getdetail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/rawdata '\n  method: post\n  operationId: rawdatav2-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/rawdata  '\n  method: post\n  operationId: rawdatav2-deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/rawdata\n  method: post\n  operationId: rawdatav2-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/signature\n\
  \  method: post\n  operationId: signaturev2-getnonce\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/sleep\n  method: post\n  operationId: sleepv2-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/sleep '\n  method: post\n  operationId: sleepv2-getsummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/stetho\n  method: post\n  operationId: stethov2-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/stetho '\n  method: post\n  operationId: stethov2-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/survey '\n  method: post\n  operationId: surveyv2-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/survey  '\n  method: post\n  operationId: surveyv2-deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/survey\n  method: post\n  operationId: surveyv2-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/survey   '\n  method:\
  \ post\n  operationId: surveyv2-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/survey    '\n  method: post\n  operationId: surveyv2-listusers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/user '\n  method: post\n  operationId: userv2-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/user      '\n  method: post\n  operationId: userv2-addtorpm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://wbsapi.withings.net/v2/user\n  method: post\n  operationId: userv2-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/user   '\n  method: post\n  operationId: userv2-getdevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/user     '\n  method: post\n  operationId: userv2-getgoals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/user  '\n  method: post\n  operationId: userv2-link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: 'https://wbsapi.withings.net/v2/user    '\n  method: post\n  operationId:\
  \ userv2-unlink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withings/refs/heads/main/agentic-access/withings-agentic-access.yml
summary_line: 62 operations · 61 acting · 3 human-in-the-loop
tags:
- Health
- Wearables
- Connected Devices
- Body Composition
- Sleep Tracking
- Blood Pressure
- Activity Tracking
- Remote Patient Monitoring
- Authentication
- Webhook
---
