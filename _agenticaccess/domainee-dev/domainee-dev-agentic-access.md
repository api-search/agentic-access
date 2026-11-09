---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 32
api_specs:
- filename: domainee-dev-dns-api-openapi.yml
  format: yaml
  label: domainee-dev DNS API
  slug: domainee-dev-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-dns-api-openapi.yml
- filename: domainee-dev-domain-purchases-api-openapi.yml
  format: yaml
  label: domainee-dev Domain purchases API
  slug: domainee-dev-domain-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-domain-purchases-api-openapi.yml
- filename: domainee-dev-domains-api-openapi.yml
  format: yaml
  label: domainee-dev Domains API
  slug: domainee-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-domains-api-openapi.yml
- filename: domainee-dev-free-tools-api-openapi.yml
  format: yaml
  label: domainee-dev Free tools API
  slug: domainee-dev-free-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-free-tools-api-openapi.yml
- filename: domainee-dev-origin-secret-api-openapi.yml
  format: yaml
  label: domainee-dev Origin secret API
  slug: domainee-dev-origin-secret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-origin-secret-api-openapi.yml
- filename: domainee-dev-projects-api-openapi.yml
  format: yaml
  label: domainee-dev Projects API
  slug: domainee-dev-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-projects-api-openapi.yml
- filename: domainee-dev-service-api-openapi.yml
  format: yaml
  label: domainee-dev Service API
  slug: domainee-dev-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-service-api-openapi.yml
- filename: domainee-dev-webhooks-api-openapi.yml
  format: yaml
  label: domainee-dev Webhooks API
  slug: domainee-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domainee-dev/openapi/domainee-dev-webhooks-api-openapi.yml
consequence_counts:
  physical: 6
  read: 32
  safety-critical: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Domainee Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/origin-secret
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domain-purchases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/domain-purchases/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domain-purchases/{id}/connect
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/domain-purchases/{id}/dns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/domain-purchases/{id}/nameservers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/domain-purchases/{id}/renew
operation_count: 51
overview: 'domainee-dev exposes 51 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 12 write, 6 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: domainee-dev
provider_slug: domainee-dev
slug: domainee-dev-agentic-access
source_filename: domainee-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/domainee-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    connected: 32\n    acting: 19\n  by_consequence:\n    read: 32\n    write: 12\n    physical: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /healthz\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/domains\n  method: post\n  operationId: createDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}\n  method: get\n  operationId: getDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{id}\n  method: patch\n  operationId: updateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}\n  method: delete\n  operationId: deleteDomain\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}/check\n  method: post\n  operationId: checkDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}/instructions\n  method: get\n  operationId: getConnectInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{id}/connect-session\n  method: post\n  operationId: createConnectSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{id}/dns/apply\n  method: post\n  operationId: applyDnsWithToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domain-purchases/check\n  method: get\n  operationId: checkDomainAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domain-purchases\n  method: get\n  operationId: listDomainPurchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v1/domain-purchases\n  method: post\n  operationId: purchaseDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domain-purchases/{id}\n  method: get\n  operationId: getDomainPurchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domain-purchases/{id}\n  method: patch\n  operationId: setDomainPurchaseAutoRenew\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domain-purchases/{id}/details\n  method: get\n  operationId: getDomainPurchaseDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domain-purchases/{id}/dns\n  method: get\n  operationId: listDomainPurchaseDnsRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domain-purchases/{id}/dns\n  method: put\n  operationId: replaceDomainPurchaseDnsRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/domain-purchases/{id}/nameservers\n  method: put\n  operationId: setDomainPurchaseNameservers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domain-purchases/{id}/renew\n  method: post\n  operationId: renewDomainPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domain-purchases/{id}/connect\n  method: post\n  operationId: connectDomainPurchase\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domain-purchases/{id}/auth-code\n  method: get\n  operationId: getDomainPurchaseAuthCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dns/check-records-exist\n  method: post\n  operationId: checkDnsRecordsExist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dns/check-records-match-exactly\n  method: post\n  operationId: checkDnsRecordsMatchExactly\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-endpoints\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints/{id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/origin-secret\n  method: get\n  operationId: getOriginSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/origin-secret\n  method: post\n  operationId: rotateOriginSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/origin-secret\n  method: delete\n  operationId: disableOriginSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/ssl-check\n\
  \  method: get\n  operationId: toolSslCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/dns-record-lookup\n  method: get\n  operationId: toolDnsRecordLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/whois-lookup\n  method: get\n  operationId: toolWhoisLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/cname-lookup\n  method: get\n  operationId: toolCnameLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/dns-provider-lookup\n  method: get\n  operationId: toolDnsProviderLookup\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/domain-connect-checker\n  method: get\n  operationId: toolDomainConnectChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/http-header-checker\n  method: get\n  operationId: toolHttpHeaderChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/dns-propagation-checker\n  method: get\n  operationId: toolDnsPropagationChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/redirect-checker\n  method: get\n  operationId: toolRedirectChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/spf-record-checker\n  method: get\n  operationId: toolSpfRecordChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/domain-age-checker\n  method: get\n  operationId: toolDomainAgeChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/subdomain-finder\n  method: get\n  operationId: toolSubdomainFinder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/reverse-ip-lookup\n  method: get\n  operationId: toolReverseIpLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/tools/dmarc-record-checker\n  method: get\n  operationId: toolDmarcRecordChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/txt-record-lookup\n  method: get\n  operationId: toolTxtRecordLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/website-status-checker\n  method: get\n  operationId: toolWebsiteStatusChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/dkim-record-checker\n  method: get\n  operationId: toolDkimRecordChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/domain-availability-checker\n\
  \  method: get\n  operationId: toolDomainAvailabilityChecker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/domainee-dev/agentic-access/domainee-dev-agentic-access.yml
summary_line: 51 operations · 19 acting · 1 human-in-the-loop
tags:
- Software-as-a-Service
- Custom Domains
- Free Tier
- MCP
---
