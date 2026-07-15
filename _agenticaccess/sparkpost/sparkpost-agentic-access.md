---
acting_count: 34
action_class_counts:
  acting: 34
  connected: 45
api_specs:
- filename: sparkpost-transmissions-openapi.yml
  format: yaml
  label: SparkPost Transmissions API
  slug: transmissions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-transmissions-openapi.yml
- filename: sparkpost-templates-openapi.yml
  format: yaml
  label: SparkPost Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-templates-openapi.yml
- filename: sparkpost-metrics-openapi.yml
  format: yaml
  label: SparkPost Metrics API
  slug: metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-metrics-openapi.yml
- filename: sparkpost-events-openapi.yml
  format: yaml
  label: SparkPost Message Events API
  slug: events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-events-openapi.yml
- filename: sparkpost-webhooks-openapi.yml
  format: yaml
  label: SparkPost Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-webhooks-openapi.yml
- filename: sparkpost-suppression-list-openapi.yml
  format: yaml
  label: SparkPost Suppression List API
  slug: suppression-list
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-suppression-list-openapi.yml
- filename: sparkpost-recipient-lists-openapi.yml
  format: yaml
  label: SparkPost Recipient Lists API
  slug: recipient-lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-recipient-lists-openapi.yml
- filename: sparkpost-sending-domains-openapi.yml
  format: yaml
  label: SparkPost Sending Domains API
  slug: sending-domains
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-sending-domains-openapi.yml
- filename: sparkpost-subaccounts-openapi.yml
  format: yaml
  label: SparkPost Subaccounts API
  slug: subaccounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-subaccounts-openapi.yml
- filename: sparkpost-inbound-openapi.yml
  format: yaml
  label: SparkPost Inbound Domains & Relay Webhooks API
  slug: inbound
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-inbound-openapi.yml
consequence_counts:
  physical: 8
  read: 45
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sparkpost Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sending-domains
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /sending-domains/{domain}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /sending-domains/{domain}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sending-domains/{domain}/dkim-keys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /sending-domains/{domain}/dkim-keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /sending-domains/{domain}/dkim-keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sending-domains/{domain}/dkim-keys/{key_id}/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sending-domains/{domain}/verify
operation_count: 79
overview: 'SparkPost exposes 79 API operations that an AI agent could call, of which 34 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read, 26 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SparkPost
provider_slug: sparkpost
slug: sparkpost-agentic-access
source_filename: sparkpost-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sparkpost-events-openapi.yml, openapi/sparkpost-inbound-openapi.yml, openapi/sparkpost-metrics-openapi.yml,\n  openapi/sparkpost-recipient-lists-openapi.yml, openapi/sparkpost-sending-domains-openapi.yml,\n  openapi/sparkpost-subaccounts-openapi.yml, openapi/sparkpost-suppression-list-openapi.yml,\n  openapi/sparkpost-templates-openapi.yml, openapi/sparkpost-transmissions-openapi.yml, openapi/sparkpost-webhooks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 79\n  by_action_class:\n    connected: 45\n    acting: 34\n  by_consequence:\n    read: 45\n    write: 26\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /events/message\n  method: get\n  operationId:\
  \ searchMessageEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/message/documentation\n  method: get\n  operationId: getMessageEventsDocumentation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/message/samples\n  method: get\n  operationId: getMessageEventSamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/ingest\n  method: get\n  operationId: searchIngestEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbound-domains\n  method: post\n  operationId: createInboundDomain\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inbound-domains\n  method: get\n  operationId: listInboundDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbound-domains/{domain}\n  method: get\n  operationId: getInboundDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbound-domains/{domain}\n  method: delete\n  operationId: deleteInboundDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /relay-webhooks\n  method: post\n  operationId: createRelayWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relay-webhooks\n  method: get\n  operationId: listRelayWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relay-webhooks/{id}\n  method: get\n  operationId: getRelayWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relay-webhooks/{id}\n  method: put\n  operationId: updateRelayWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relay-webhooks/{id}\n  method: delete\n  operationId: deleteRelayWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relay-webhooks/{id}/validate\n  method: post\n  operationId: validateRelayWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/\n  method: get\n  operationId: getMetricsRoot\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability\n  method: get\n  operationId: getMetricsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/query-filters-schema\n  method: get\n  operationId: getQueryFiltersSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/domain\n  method: get\n  operationId: getMetricsByDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/sending-ip\n  method: get\n  operationId: getMetricsBySendingIP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/ip-pool\n  method: get\n  operationId: getMetricsByIPPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/sending-domain\n  method: get\n  operationId: getMetricsBySendingDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/subaccount\n  method: get\n  operationId: getMetricsBySubaccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/campaign\n  method: get\n  operationId: getMetricsByCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/template\n  method: get\n  operationId: getMetricsByTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/watched-domain\n  method: get\n  operationId: getMetricsByWatchedDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/mailbox-provider\n  method: get\n  operationId: getMetricsByMailboxProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/mailbox-provider-region\n  method: get\n  operationId: getMetricsByMailboxProviderRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/time-series\n  method: get\n  operationId: getMetricsTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/bounce-reason\n  method: get\n  operationId: getMetricsByBounceReason\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/bounce-reason/domain\n  method: get\n  operationId: getMetricsByBounceReasonDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/deliverability/subject-campaign\n  method: get\n  operationId: getMetricsBySubjectCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipient-lists\n  method: post\n  operationId: createRecipientList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipient-lists\n  method: get\n  operationId: listRecipientLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipient-lists/{id}\n  method: get\n  operationId: getRecipientList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipient-lists/{id}\n  method: put\n  operationId: updateRecipientList\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipient-lists/{id}\n  method: delete\n  operationId: deleteRecipientList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sending-domains\n  method: post\n  operationId: createSendingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sending-domains\n\
  \  method: get\n  operationId: listSendingDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sending-domains/{domain}\n  method: get\n  operationId: getSendingDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sending-domains/{domain}\n  method: put\n  operationId: updateSendingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sending-domains/{domain}\n  method: delete\n  operationId: deleteSendingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sending-domains/{domain}/verify\n  method: post\n  operationId: verifySendingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sending-domains/{domain}/dkim-keys\n  method: get\n  operationId: listDkimKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sending-domains/{domain}/dkim-keys\n  method: post\n  operationId: createDkimKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sending-domains/{domain}/dkim-keys/{key_id}\n  method: get\n  operationId: getDkimKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sending-domains/{domain}/dkim-keys/{key_id}\n  method: put\n  operationId: updateDkimKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /sending-domains/{domain}/dkim-keys/{key_id}\n  method: delete\n  operationId: deleteDkimKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sending-domains/{domain}/dkim-keys/{key_id}/verify\n  method: post\n  operationId: verifyDkimKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subaccounts\n  method: post\n  operationId: createSubaccount\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subaccounts\n  method: get\n  operationId: listSubaccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subaccounts/summary\n  method: get\n  operationId: getSubaccountsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subaccounts/{id}\n  method: get\n  operationId: getSubaccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subaccounts/{id}\n  method: put\n  operationId: updateSubaccount\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suppression-list\n  method: put\n  operationId: bulkUpsertSuppressions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suppression-list\n  method: get\n  operationId: searchSuppressions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suppression-list/summary\n  method: get\n  operationId: getSuppressionSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /suppression-list/{recipient}\n  method: put\n  operationId: upsertSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suppression-list/{recipient}\n  method: get\n  operationId: getSuppression\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suppression-list/{recipient}\n  method: delete\n  operationId: deleteSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /templates\n  method: post\n  operationId: createTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/{id}\n  method: get\n  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/{id}\n  method: put\n  operationId: updateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /templates/{id}\n  method: delete\n  operationId: deleteTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /templates/{id}/preview\n  method: post\n  operationId: previewTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /utils/content-previewer\n  method: post\n  operationId: previewInlineTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transmissions\n  method: post\n  operationId: createTransmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transmissions\n  method: delete\n  operationId: deleteTransmissionsByCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transmissions/{id}\n  method: get\n  operationId: getTransmission\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transmissions/{id}\n  method: delete\n  operationId: deleteTransmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/validate\n  method:\
  \ post\n  operationId: validateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/batch-status\n  method: get\n  operationId: getWebhookBatchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/events/documentation\n  method: get\n  operationId: getWebhookEventsDocumentation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/events/samples\n  method: get\n  operationId: getWebhookEventSamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/agentic-access/sparkpost-agentic-access.yml
summary_line: 79 operations · 34 acting
tags:
- Email
- Transactional Email
- Marketing Email
- Email Delivery
- SMTP
- Webhooks
- Analytics
- Templates
- Suppression List
---
