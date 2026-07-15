---
acting_count: 782
action_class_counts:
  acting: 782
  connected: 460
api_specs:
- filename: kong-gateway-admin-api.yml
  format: yaml
  label: Kong Gateway Admin API
  slug: kong-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/openapi/kong-gateway-admin-api.yml
- filename: kong-konnect-platform-api.yml
  format: yaml
  label: Kong Konnect Platform API
  slug: kong-konnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/openapi/kong-konnect-platform-api.yml
- filename: openapi.yaml
  format: yaml
  label: Kong Event Gateway
  slug: kong-event-gateway
  spec_type: OpenAPI
  url: https://developer.konghq.com/api/konnect/event-gateway/v1/
consequence_counts:
  physical: 8
  read: 460
  safety-critical: 122
  write: 652
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 122
kind: agentic-access
layout: agentic-access
method: generated
name: Kong Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/mcp-cp/{controlPlaneId}/mcp-servers/{mcpServerId}/status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/control-planes
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v2/control-planes/{controlPlaneId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/control-planes/{controlPlaneId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/control-planes/{controlPlaneId}/config-stores
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/control-planes/{controlPlaneId}/config-stores/{configStoreId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/control-planes/{controlPlaneId}/config-stores/{configStoreId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/control-planes/{controlPlaneId}/config-stores/{configStoreId}/secrets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/control-planes/{controlPlaneId}/config-stores/{configStoreId}/secrets/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/control-planes/{controlPlaneId}/config-stores/{configStoreId}/secrets/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/control-planes/{controlPlaneId}/core-entities/ca_certificates
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/control-planes/{controlPlaneId}/core-entities/ca_certificates/{CACertificateId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/control-planes/{controlPlaneId}/core-entities/ca_certificates/{CACertificateId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/control-planes/{controlPlaneId}/core-entities/certificates
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/control-planes/{controlPlaneId}/core-entities/certificates/{CertificateId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/control-planes/{controlPlaneId}/core-entities/certificates/{CertificateId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/control-planes/{controlPlaneId}/core-entities/certificates/{CertificateId}/snis
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/control-planes/{controlPlaneId}/core-entities/certificates/{CertificateId}/snis/{SNIId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/control-planes/{controlPlaneId}/core-entities/certificates/{CertificateId}/snis/{SNIId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/control-planes/{controlPlaneId}/core-entities/consumer_groups
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/control-planes/{controlPlaneId}/core-entities/consumer_groups/{ConsumerGroupId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/control-planes/{controlPlaneId}/core-entities/consumer_groups/{ConsumerGroupId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/control-planes/{controlPlaneId}/core-entities/consumer_groups/{ConsumerGroupId}/consumers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/control-planes/{controlPlaneId}/core-entities/consumer_groups/{ConsumerGroupId}/consumers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/control-planes/{controlPlaneId}/core-entities/consumer_groups/{ConsumerGroupId}/consumers/{ConsumerId}
operation_count: 1242
overview: 'Kong exposes 1242 API operations that an AI agent could call, of which 782 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 460 read, 652 write, 8 physical, and 122 safety-critical.


  122 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kong
provider_slug: kong
slug: kong-agentic-access
source_filename: kong-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kong-gateway-admin-api.yml, openapi/kong-konnect-platform-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1242\n  by_action_class:\n    acting: 782\n    connected: 460\n  by_consequence:\n    write: 652\n    read: 460\n    safety-critical: 122\n    physical: 8\n  human_in_the_loop_required: 122\noperations:\n- path: /{workspace}/certificates\n  method: post\n  operationId: create-certificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/certificates/{CertificateId}\n\
  \  method: delete\n  operationId: delete-certificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/certificates/{CertificateId}\n  method: get\n  operationId: get-certificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/certificates/{CertificateId}\n  method: put\n  operationId: upsert-certificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumer_groups\n  method:\
  \ post\n  operationId: create-consumer_group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumer_groups/{ConsumerGroupId}\n  method: delete\n  operationId: delete-consumer_group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumer_groups/{ConsumerGroupId}\n  method: get\n  operationId: get-consumer_group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/consumer_groups/{ConsumerGroupId}\n\
  \  method: put\n  operationId: upsert-consumer_group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumer_groups/{ConsumerGroupId}/consumers\n  method: post\n  operationId: add-consumer-to-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumer_groups/{ConsumerGroupId}/consumers/{ConsumerIdOrUsername}\n  method: delete\n  operationId: remove-consumer-from-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers\n  method: post\n  operationId: create-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/acls\n  method: post\n  operationId: create-acl-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/acls/{ACLId}\n  method: delete\n\
  \  operationId: delete-acl-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/acls/{ACLId}\n  method: get\n  operationId: get-acl-with-consumer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/basic-auth\n  method: post\n  operationId: create-basic-auth-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/basic-auth/{BasicAuthId}\n  method: delete\n  operationId: delete-basic-auth-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/basic-auth/{BasicAuthId}\n  method: get\n  operationId: get-basic-auth-with-consumer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/hmac-auth\n  method: post\n  operationId: create-hmac-auth-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/hmac-auth/{HMACAuthId}\n  method: delete\n  operationId: delete-hmac-auth-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/hmac-auth/{HMACAuthId}\n  method: get\n  operationId: get-hmac-auth-with-consumer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/jwt\n  method: post\n  operationId: create-jwt-with-consumer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/jwt/{JWTId}\n  method: delete\n  operationId: delete-jwt-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/jwt/{JWTId}\n  method: get\n  operationId: get-jwt-with-consumer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/key-auth\n  method:\
  \ post\n  operationId: create-key-auth-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/key-auth/{KeyAuthId}\n  method: delete\n  operationId: delete-key-auth-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/key-auth/{KeyAuthId}\n  method: get\n  operationId: get-key-auth-with-consumer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/mtls-auth\n  method: post\n  operationId: create-mtls-auth-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/mtls-auth/{MTLSAuthId}\n  method: delete\n  operationId: delete-mtls-auth-with-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdForNestedEntities}/mtls-auth/{MTLSAuthId}\n  method: get\n  operationId: get-mtls-auth-with-consumer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/consumers/{ConsumerIdOrUsername}\n  method: delete\n  operationId: delete-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/consumers/{ConsumerIdOrUsername}\n  method: get\n  operationId: get-consumer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/consumers/{ConsumerIdOrUsername}\n  method: put\n  operationId: upsert-consumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/key-sets\n  method: post\n  operationId: create-key-set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/key-sets/{KeySetIdOrName}\n  method: delete\n  operationId: delete-key-set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/key-sets/{KeySetIdOrName}\n  method: get\n  operationId: get-key-set\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/key-sets/{KeySetIdOrName}\n  method: put\n  operationId: upsert-key-set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/keys\n  method: post\n  operationId: create-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/keys/{KeyIdOrName}\n  method: delete\n  operationId: delete-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/keys/{KeyIdOrName}\n  method: get\n  operationId: get-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/keys/{KeyIdOrName}\n  method: put\n  operationId: upsert-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/partials\n  method: post\n  operationId: create-partial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/partials/{PartialId}\n  method: delete\n  operationId: delete-partial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/partials/{PartialId}\n  method: get\n  operationId: get-partial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/partials/{PartialId}\n  method: put\n  operationId: upsert-partial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins\n  method: get\n  operationId: list-plugin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{workspace}/plugins\n  method: post\n  operationId: create-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#ACL\n  method: post\n  operationId: create-acl-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /{workspace}/plugins#Ace\n  method: post\n  operationId: create-ace-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#Acme\n  method: post\n  operationId: create-acme-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiA2aProxy\n  method: post\n  operationId: create-aia2aproxy-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiAwsGuardrails\n  method: post\n  operationId: create-aiawsguardrails-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiAzureContentSafety\n  method: post\n  operationId: create-aiazurecontentsafety-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{workspace}/plugins#AiCustomGuardrail\n  method: post\n  operationId:\
  \ create-aicustomguardrail-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiGcpModelArmor\n  method: post\n  operationId: create-aigcpmodelarmor-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiLakeraGuard\n  method: post\n  operationId: create-ailakeraguard-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiLlmAsJudge\n  method: post\n  operationId: create-aillmasjudge-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiMcpOauth2\n  method: post\n  operationId: create-aimcpoauth2-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiMcpProxy\n  method: post\n  operationId: create-aimcpproxy-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiPromptCompressor\n  method: post\n  operationId: create-aipromptcompressor-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiPromptDecorator\n  method: post\n  operationId: create-aipromptdecorator-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiPromptGuard\n\
  \  method: post\n  operationId: create-aipromptguard-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiPromptTemplate\n  method: post\n  operationId: create-aiprompttemplate-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiProxy\n  method: post\n  operationId: create-aiproxy-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiProxyAdvanced\n  method: post\n  operationId: create-aiproxyadvanced-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiRagInjector\n  method: post\n  operationId: create-airaginjector-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiRateLimitingAdvanced\n  method: post\n  operationId: create-airatelimitingadvanced-plugin\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiRequestTransformer\n  method: post\n  operationId: create-airequesttransformer-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiResponseTransformer\n  method: post\n  operationId: create-airesponsetransformer-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiSanitizer\n  method: post\n  operationId: create-aisanitizer-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiSemanticCache\n  method: post\n  operationId: create-aisemanticcache-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiSemanticPromptGuard\n  method: post\n  operationId: create-aisemanticpromptguard-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AiSemanticResponseGuard\n  method: post\n  operationId: create-aisemanticresponseguard-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AppDynamics\n  method: post\n  operationId: create-appdynamics-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AwsLambda\n\
  \  method: post\n  operationId: create-awslambda-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#AzureFunctions\n  method: post\n  operationId: create-azurefunctions-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#BasicAuth\n  method: post\n  operationId: create-basicauth-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#BotDetection\n  method: post\n  operationId: create-botdetection-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#Canary\n  method: post\n  operationId: create-canary-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#Confluent\n  method: post\n  operationId: create-confluent-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#ConfluentConsume\n  method: post\n  operationId: create-confluentconsume-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#CorrelationId\n  method: post\n  operationId: create-correlationid-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#Cors\n\
  \  method: post\n  operationId: create-cors-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#Datadog\n  method: post\n  operationId: create-datadog-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#Datakit\n  method: post\n  operationId: create-datakit-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#Degraphql\n  method: post\n  operationId: create-degraphql-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#ExitTransformer\n  method: post\n  operationId: create-exittransformer-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#FileLog\n  method: post\n  operationId: create-filelog-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#ForwardProxy\n  method: post\n  operationId: create-forwardproxy-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#GraphqlProxyCacheAdvanced\n  method: post\n  operationId: create-graphqlproxycacheadvanced-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#GraphqlRateLimitingAdvanced\n\
  \  method: post\n  operationId: create-graphqlratelimitingadvanced-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#GrpcGateway\n  method: post\n  operationId: create-grpcgateway-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{workspace}/plugins#GrpcWeb\n  method: post\n  operationId: create-grpcweb-plugin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\n\n# --- truncated at 32 KB (407 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/agentic-access/kong-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/agentic-access/kong-agentic-access.yml
summary_line: 1242 operations · 782 acting · 122 human-in-the-loop
tags:
- API Gateway
- AI Gateway
- AI Connectivity
- Agent Gateway
- Event Gateway
- MCP Registry
- Service Mesh
- LLM
- Kafka
- Konnect
- Open Source
---
