---
acting_count: 219
action_class_counts:
  acting: 219
  connected: 119
api_specs:
- filename: exoscale-openapi.yml
  format: yaml
  label: Exoscale API
  slug: exoscale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exoscale/refs/heads/main/openapi/exoscale-openapi.yml
consequence_counts:
  physical: 4
  read: 119
  safety-critical: 24
  write: 191
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 24
kind: agentic-access
layout: agentic-access
method: generated
name: Exoscale Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dbaas-grafana/{service-name}/user/{username}/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dbaas-kafka/{service-name}/user/{username}/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dbaas-mysql/{name}/migration/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dbaas-mysql/{service-name}/user/{username}/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dbaas-opensearch/{service-name}/user/{username}/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dbaas-postgres/{name}/migration/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dbaas-postgres/{service-name}/user/{username}/allow-replication
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dbaas-postgres/{service-name}/user/{username}/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dbaas-valkey/{name}/migration/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dbaas-valkey/{service-name}/user/{username}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /dbaas-valkey/{service-name}/user/{username}/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /elastic-ip/{id}/{field}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /iam-organization-policy:reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /instance-pool/{id}/{field}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /instance/{id}/{field}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /instance/{id}:reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /instance/{id}:reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /instance/{id}:reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /instance/{id}:stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /kms-key/{id}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /kms-key/{id}/disable-key-rotation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /load-balancer/{id}/service/{service-id}/{field}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /load-balancer/{id}/{field}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /private-network/{id}/{field}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ai/deployment
operation_count: 338
overview: 'Exoscale exposes 338 API operations that an AI agent could call, of which 219 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 119 read, 191 write, 4 physical, and 24 safety-critical.


  24 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Exoscale
provider_slug: exoscale
slug: exoscale-agentic-access
source_filename: exoscale-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/exoscale-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 338\n  by_action_class:\n    acting: 219\n    connected: 119\n  by_consequence:\n    write: 191\n    read: 119\n    safety-critical: 24\n    physical: 4\n  human_in_the_loop_required: 24\noperations:\n- path: /load-balancer/{id}/service/{service-id}\n  method: delete\n  operationId: delete-load-balancer-service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /load-balancer/{id}/service/{service-id}\n\
  \  method: put\n  operationId: update-load-balancer-service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /load-balancer/{id}/service/{service-id}\n  method: get\n  operationId: get-load-balancer-service\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-external-endpoint-opensearch/{endpoint-id}\n  method: delete\n  operationId: delete-dbaas-external-endpoint-opensearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /dbaas-external-endpoint-opensearch/{endpoint-id}\n  method: get\n  operationId: get-dbaas-external-endpoint-opensearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-external-endpoint-opensearch/{endpoint-id}\n  method: put\n  operationId: update-dbaas-external-endpoint-opensearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-opensearch/{name}/acl-config\n  method: get\n  operationId: get-dbaas-opensearch-acl-config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-opensearch/{name}/acl-config\n  method: put\n \
  \ operationId: update-dbaas-opensearch-acl-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instance-pool/{id}:scale\n  method: put\n  operationId: scale-instance-pool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instance/{id}:create-snapshot\n  method: post\n  operationId: create-snapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-valkey/{name}/migration/stop\n  method: post\n  operationId: stop-dbaas-valkey-migration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reverse-dns/elastic-ip/{id}\n  method: get\n  operationId: get-reverse-dns-elastic-ip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse-dns/elastic-ip/{id}\n  method: post\n  operationId: update-reverse-dns-elastic-ip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reverse-dns/elastic-ip/{id}\n  method: delete\n  operationId: delete-reverse-dns-elastic-ip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /anti-affinity-group\n  method: get\n  operationId: list-anti-affinity-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /anti-affinity-group\n  method: post\n  operationId: create-anti-affinity-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /ai/ai-api-key\n  method: get\n  operationId: list-ai-api-keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/ai-api-key\n  method: post\n  operationId: create-ai-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usage-report\n  method: get\n  operationId: get-usage-report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event\n  method: get\n  operationId: list-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /security-group/{id}/rules/{rule-id}\n  method: delete\n  operationId: delete-rule-from-security-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-grafana/{name}/maintenance/start\n  method: put\n  operationId: start-dbaas-grafana-maintenance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kms-key/{id}/disable-key-rotation\n  method: post\n  operationId: disable-kms-key-rotation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dbaas-postgres/{service}/upgrade-check\n  method: post\n  operationId: create-dbaas-pg-upgrade-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-mysql/{service-name}/user/{username}/password/reset\n  method: put\n  operationId: reset-dbaas-mysql-user-password\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /ai/help/inference-engine-parameters\n  method: get\n  operationId: get-inference-engine-help\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /load-balancer\n  method: post\n  operationId: create-load-balancer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /load-balancer\n  method: get\n  operationId: list-load-balancers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security-group\n  method: post\n  operationId: create-security-group\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security-group\n  method: get\n  operationId: list-security-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-postgres/{service-name}/connection-pool\n  method: post\n  operationId: create-dbaas-pg-connection-pool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-mysql/{name}\n  method: put\n  operationId: update-dbaas-service-mysql\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-mysql/{name}\n  method: get\n  operationId: get-dbaas-service-mysql\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-mysql/{name}\n  method: post\n  operationId: create-dbaas-service-mysql\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-mysql/{name}\n  method: delete\n  operationId: delete-dbaas-service-mysql\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam-role/{target-role-id}/assume\n  method: post\n  operationId: assume-iam-role\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /private-network/{id}:attach\n  method: put\n  operationId: attach-instance-to-private-network\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kms-key/{id}\n  method: get\n  operationId: get-kms-key\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-thanos/{name}/maintenance/start\n  method: put\n  operationId: start-dbaas-thanos-maintenance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-external-endpoint-elasticsearch/{endpoint-id}\n  method: delete\n  operationId: delete-dbaas-external-endpoint-elasticsearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-external-endpoint-elasticsearch/{endpoint-id}\n  method:\
  \ get\n  operationId: get-dbaas-external-endpoint-elasticsearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-external-endpoint-elasticsearch/{endpoint-id}\n  method: put\n  operationId: update-dbaas-external-endpoint-elasticsearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/model\n  method: post\n  operationId: create-model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/model\n  method: get\n\
  \  operationId: list-models\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-mysql/{service-name}/user\n  method: post\n  operationId: create-dbaas-mysql-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-service-type\n  method: get\n  operationId: list-dbaas-service-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/deployment/{id}/scale\n  method: post\n  operationId: scale-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instance-type/{id}\n  method: get\n  operationId: get-instance-type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance/{id}:password\n  method: get\n  operationId: reveal-instance-password\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sks-template/{kube-version}/{variant}\n  method: get\n  operationId: get-active-nodepool-template\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance/{id}:resize-disk\n  method: put\n  operationId: resize-instance-disk\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-service\n  method: get\n  operationId: list-dbaas-services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elastic-ip\n  method: post\n  operationId: create-elastic-ip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /elastic-ip\n  method: get\n  operationId: list-elastic-ips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zone\n  method: get\n  operationId: list-zones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance-pool\n  method: get\n  operationId: list-instance-pools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance-pool\n  method: post\n  operationId: create-instance-pool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-external-endpoint-rsyslog/{name}\n  method: post\n  operationId: create-dbaas-external-endpoint-rsyslog\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sks-cluster-kubeconfig/{id}\n  method: post\n  operationId: generate-sks-cluster-kubeconfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns-domain/{domain-id}/record\n  method: get\n  operationId: list-dns-domain-records\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns-domain/{domain-id}/record\n  method: post\n  operationId: create-dns-domain-record\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-ca-certificate\n  method: get\n  operationId: get-dbaas-ca-certificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-settings-grafana\n  method: get\n  operationId: get-dbaas-settings-grafana\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deploy-target\n  method: get\n  operationId: list-deploy-targets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance-type\n  method: get\n  operationId: list-instance-types\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/deployment\n  method: post\n  operationId: create-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/deployment\n  method: get\n  operationId: list-deployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-postgres/{service-name}/database/{database-name}\n  method: delete\n  operationId: delete-dbaas-pg-database\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /block-storage/{id}:attach\n  method: put\n  operationId: attach-block-storage-volume-to-instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kms-key/{id}/enable\n  method: post\n  operationId: enable-kms-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-postgres/{name}/migration/stop\n  method: post\n  operationId: stop-dbaas-pg-migration\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dbaas-kafka/{name}\n  method: get\n  operationId: get-dbaas-service-kafka\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-kafka/{name}\n  method: post\n  operationId: create-dbaas-service-kafka\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-kafka/{name}\n  method: put\n  operationId: update-dbaas-service-kafka\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-kafka/{name}\n  method: delete\n  operationId: delete-dbaas-service-kafka\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instance/{id}:reset-password\n  method: put\n  operationId: reset-instance-password\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /dbaas-kafka/{name}/schema-registry/acl-config\n  method: post\n  operationId: create-dbaas-kafka-schema-registry-acl-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /private-network/{id}:update-ip\n  method: put\n  operationId: update-private-network-instance-ip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sks-cluster/{id}/nodepool/{sks-nodepool-id}\n  method: put\n  operationId: update-sks-nodepool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sks-cluster/{id}/nodepool/{sks-nodepool-id}\n  method: get\n  operationId: get-sks-nodepool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sks-cluster/{id}/nodepool/{sks-nodepool-id}\n  method: delete\n  operationId: delete-sks-nodepool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /block-storage-snapshot/{id}\n  method: delete\n  operationId: delete-block-storage-snapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /block-storage-snapshot/{id}\n  method: put\n  operationId: update-block-storage-snapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /block-storage-snapshot/{id}\n  method: get\n  operationId: get-block-storage-snapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kms-key/{id}/list-key-rotations\n  method: get\n  operationId: list-kms-key-rotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-postgres/{service-name}/user\n  method: post\n  operationId: create-dbaas-postgres-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-external-integrations/{service-name}\n  method: get\n  operationId: list-dbaas-external-integrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbaas-external-integration/{integration-id}\n  method: get\n  operationId: get-dbaas-external-integration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance-pool/{id}\n  method:\
  \ delete\n  operationId: delete-instance-pool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instance-pool/{id}\n  method: get\n  operationId: get-instance-pool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance-pool/{id}\n  method: put\n  operationId: update-instance-pool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-external-endpoint-types\n  method: get\n  operationId: list-dbaas-external-endpoint-types\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private-network\n  method: get\n  operationId: list-private-networks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /private-network\n  method: post\n  operationId: create-private-network\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instance/{id}:start\n  method: put\n  operationId: start-instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instance/{id}:enable-tpm\n  method: post\n  operationId: enable-tpm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization\n  method: get\n  operationId: get-organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security-group/{id}\n  method: get\n  operationId: get-security-group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security-group/{id}\n  method: delete\n  operationId: delete-security-group\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sks-cluster/{id}/authority/{authority}/cert\n  method: get\n  operationId: get-sks-cluster-authority-cert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snapshot/{id}:export\n  method: post\n  operationId: export-snapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/deployment/{id}\n  method: get\n  operationId: get-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/deployment/{id}\n  method: patch\n  operationId: update-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/deployment/{id}\n  method: delete\n  operationId: delete-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbaas-kafka/{service-name}/connect/password/reveal\n  method: get\n  operationId: reveal-dbaas-kafka-connect-password\n\
  \  x-agentic-access:\n    action-class: connected\n    cons\n\n# --- truncated at 32 KB (104 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/exoscale/refs/heads/main/agentic-access/exoscale-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exoscale/refs/heads/main/agentic-access/exoscale-agentic-access.yml
summary_line: 338 operations · 219 acting · 24 human-in-the-loop
tags:
- Cloud
- Infrastructure
- Compute
- Storage
- Kubernetes
- DBaaS
- Europe
---
