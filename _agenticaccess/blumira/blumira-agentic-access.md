---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 41
api_specs:
- filename: blumira-health-api-openapi.yml
  format: yaml
  label: Blumira Health API
  slug: blumira-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-health-api-openapi.yml
- filename: blumira-msp-api-openapi.yml
  format: yaml
  label: Blumira Msp API
  slug: blumira-msp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-msp-api-openapi.yml
- filename: blumira-org-api-openapi.yml
  format: yaml
  label: Blumira Org API
  slug: blumira-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-org-api-openapi.yml
- filename: blumira-resolutions-api-openapi.yml
  format: yaml
  label: Blumira Resolutions API
  slug: blumira-resolutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/openapi/blumira-resolutions-api-openapi.yml
consequence_counts:
  read: 41
  safety-critical: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 18
kind: agentic-access
layout: agentic-access
method: generated
name: Blumira Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /msp/accounts/{account_id}/agents/devices/{device_id}/actions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /msp/accounts/{account_id}/findings/{finding_id}/assign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /msp/accounts/{account_id}/findings/{finding_id}/comments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /msp/accounts/{account_id}/findings/{finding_id}/resolve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /msp/webhooks
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /msp/webhooks/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /msp/webhooks/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /msp/webhooks/{id}/rotate-secret
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /msp/webhooks/{id}/test
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /org/agents/devices/{device_id}/actions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /org/findings/{finding_id}/assign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /org/findings/{finding_id}/comments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /org/findings/{finding_id}/resolve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /org/webhooks
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /org/webhooks/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /org/webhooks/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /org/webhooks/{id}/rotate-secret
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /org/webhooks/{id}/test
operation_count: 59
overview: 'Blumira exposes 59 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 read and 18 safety-critical.


  18 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blumira
provider_slug: blumira
slug: blumira-agentic-access
source_filename: blumira-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: generated\nsource: openapi/blumira-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 59\n  by_action_class:\n    connected: 41\n    acting: 18\n  by_consequence:\n    read: 41\n    safety-critical: 18\n  human_in_the_loop_required: 18\noperations:\n- path: /health\n  method: get\n  operationId: api.controller.health.search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts\n  method: get\n  operationId: api.controller.msp.get_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /msp/accounts/findings\n  method: get\n  operationId: api.controller.msp.get_accounts_findings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}\n  method: get\n  operationId: api.controller.msp.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/agents/actions/{command_id}\n  method: get\n  operationId: api.controller.msp.get_account_agent_action\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/agents/devices\n  method: get\n  operationId: api.controller.msp.get_account_agents_devices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/agents/devices/{device_id}\n  method: get\n  operationId: api.controller.msp.get_agents_device\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/agents/devices/{device_id}/actions\n  method: post\n  operationId: api.controller.msp.dispatch_account_agent_action\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /msp/accounts/{account_id}/agents/keys\n  method: get\n  operationId: api.controller.msp.get_account_agents_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/agents/keys/{key_id}\n  method: get\n  operationId: api.controller.msp.get_agents_key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/detection-rules\n  method: get\n  operationId: api.controller.msp.get_detection_rules_by_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/detection-rules/{rule_id}\n  method: get\n  operationId: api.controller.msp.get_detection_rule_by_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/findings\n  method: get\n  operationId: api.controller.msp.get_account_findings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/findings/{finding_id}\n  method: get\n  operationId: api.controller.msp.get_account_finding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/findings/{finding_id}/assign\n  method: post\n  operationId: api.controller.msp.set_finding_owners\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /msp/accounts/{account_id}/findings/{finding_id}/comments\n  method: get\n  operationId: api.controller.msp.get_account_finding_comments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/findings/{finding_id}/comments\n  method: post\n  operationId: api.controller.msp.add_account_finding_comment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /msp/accounts/{account_id}/findings/{finding_id}/evidence\n  method: get\n  operationId: api.controller.msp.get_account_finding_evidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/accounts/{account_id}/findings/{finding_id}/resolve\n  method: post\n  operationId: api.controller.msp.resolve_finding\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /msp/accounts/{account_id}/users\n  method: get\n  operationId: api.controller.msp.list_users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/basis-detection-rules\n  method: get\n  operationId: api.controller.msp.get_msp_detection_rules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/basis-detection-rules/{rule_id}\n  method: get\n  operationId: api.controller.msp.get_msp_detection_rule\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/webhooks\n  method: get\n  operationId: api.controller.webhooks_resource.get_endpoints_msp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/webhooks\n  method: post\n  operationId: api.controller.webhooks_resource.create_endpoint_msp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /msp/webhooks/{id}\n  method: delete\n  operationId: api.controller.webhooks_resource.delete_endpoint_msp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /msp/webhooks/{id}\n  method: get\n  operationId: api.controller.webhooks_resource.get_endpoint_msp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/webhooks/{id}\n  method: put\n  operationId: api.controller.webhooks_resource.update_endpoint_msp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /msp/webhooks/{id}/deliveries\n  method: get\n  operationId: api.controller.webhooks_resource.get_deliveries_msp\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/webhooks/{id}/deliveries/{delivery_id}\n  method: get\n  operationId: api.controller.webhooks_resource.get_delivery_msp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msp/webhooks/{id}/rotate-secret\n  method: post\n  operationId: api.controller.webhooks_resource.rotate_secret_msp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /msp/webhooks/{id}/test\n  method: post\n  operationId: api.controller.webhooks_resource.test_endpoint_msp\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/agents/actions\n  method: get\n  operationId: api.controller.direct_org.get_action_catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/agents/actions/{command_id}\n  method: get\n  operationId: api.controller.direct_org.get_action_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/agents/devices\n  method: get\n  operationId: api.controller.direct_org.get_agents_devices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /org/agents/devices/{device_id}\n  method: get\n  operationId: api.controller.direct_org.get_agents_device\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/agents/devices/{device_id}/actions\n  method: post\n  operationId: api.controller.direct_org.dispatch_action_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/agents/keys\n  method: get\n  operationId: api.controller.direct_org.get_agents_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /org/agents/keys/{key_id}\n  method: get\n  operationId: api.controller.direct_org.get_agents_key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/detection-rules\n  method: get\n  operationId: api.controller.direct_org.get_detection_rules_by_org\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/detection-rules/{rule_id}\n  method: get\n  operationId: api.controller.direct_org.get_detection_rule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/findings\n  method: get\n  operationId: api.controller.direct_org.get_by_org\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /org/findings/{finding_id}\n  method: get\n  operationId: api.controller.direct_org.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/findings/{finding_id}/assign\n  method: post\n  operationId: api.controller.direct_org.set_owners\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/findings/{finding_id}/comments\n  method: get\n  operationId: api.controller.direct_org.get_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/findings/{finding_id}/comments\n  method: post\n\
  \  operationId: api.controller.direct_org.add_comment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/findings/{finding_id}/details\n  method: get\n  operationId: api.controller.direct_org.get_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/findings/{finding_id}/evidence\n  method: get\n  operationId: api.controller.direct_org.get_evidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/findings/{finding_id}/resolve\n  method: post\n  operationId: api.controller.direct_org.resolve_finding\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/users\n  method: get\n  operationId: api.controller.direct_org.list_users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/webhooks\n  method: get\n  operationId: api.controller.webhooks_resource.get_endpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/webhooks\n  method: post\n  operationId: api.controller.webhooks_resource.create_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/webhooks/{id}\n  method: delete\n  operationId: api.controller.webhooks_resource.delete_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/webhooks/{id}\n  method: get\n  operationId: api.controller.webhooks_resource.get_endpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/webhooks/{id}\n  method: put\n  operationId: api.controller.webhooks_resource.update_endpoint\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/webhooks/{id}/deliveries\n  method: get\n  operationId: api.controller.webhooks_resource.get_deliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/webhooks/{id}/deliveries/{delivery_id}\n  method: get\n  operationId: api.controller.webhooks_resource.get_delivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/webhooks/{id}/rotate-secret\n  method: post\n  operationId: api.controller.webhooks_resource.rotate_secret\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/webhooks/{id}/test\n  method: post\n  operationId: api.controller.webhooks_resource.test_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resolutions\n  method: get\n  operationId: api.controller.resolutions.get_resolutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blumira/refs/heads/main/agentic-access/blumira-agentic-access.yml
summary_line: 59 operations · 18 acting · 18 human-in-the-loop
tags:
- Company
- Security
- SaaS
- Cloud
- IT
---
