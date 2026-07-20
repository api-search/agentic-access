---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 42
api_specs:
- filename: domaintools-iris-openapi.yml
  format: yaml
  label: DomainTools Iris API
  slug: domaintools-iris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-iris-openapi.yml
- filename: domaintools-lookups-monitors-openapi.yml
  format: yaml
  label: DomainTools Lookups and Monitors API
  slug: domaintools-lookups-and-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-lookups-monitors-openapi.yml
- filename: domaintools-dnsdb-openapi.yml
  format: yaml
  label: Farsight DNSDB Passive DNS API
  slug: farsight-dnsdb-passive-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-dnsdb-openapi.yml
- filename: domaintools-sie-openapi.yml
  format: yaml
  label: Farsight SIE Batch API
  slug: farsight-sie-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-sie-openapi.yml
consequence_counts:
  read: 42
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Domaintools Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/iris-detect/monitors/
operation_count: 53
overview: 'DomainTools exposes 53 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 42 read, 10 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DomainTools
provider_slug: domaintools
slug: domaintools-agentic-access
source_filename: domaintools-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/domaintools-dnsdb-openapi.yml, openapi/domaintools-iris-openapi.yml, openapi/domaintools-lookups-monitors-openapi.yml,\n  openapi/domaintools-sie-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 42\n    acting: 11\n  by_consequence:\n    read: 42\n    write: 10\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rate_limit\n  method: get\n  operationId: getRateLimit\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/rrset/{type}/{value}\n  method: get\n  operationId: lookupRrset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/rrset/{type}/{value}/{rrtype}\n  method: get\n  operationId: lookupRrsetByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/rrset/{type}/{value}/{rrtype}/{bailiwick}\n  method: get\n  operationId: lookupRrsetByTypeAndBailiwick\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/rdata/{type}/{value}\n  method: get\n  operationId: lookupRdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/rdata/{type}/{value}/{rrtype}\n  method: get\n  operationId: lookupRdataByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summarize/rrset/{type}/{value}\n  method: get\n  operationId: summarizeRrset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summarize/rrset/{type}/{value}/{rrtype}\n  method: get\n  operationId: summarizeRrsetByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summarize/rrset/{type}/{value}/{rrtype}/{bailiwick}\n  method: get\n  operationId: summarizeRrsetByTypeAndBailiwick\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /summarize/rdata/{type}/{value}\n  method: get\n  operationId: summarizeRdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summarize/rdata/{type}/{value}/{rrtype}\n  method: get\n  operationId: summarizeRdataByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{method}/{key}/{value}\n  method: get\n  operationId: flexSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{method}/{key}/{value}/{rrtype}\n  method: get\n  operationId: flexSearchByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/iris-detect/domains/\n\
  \  method: patch\n  operationId: patchDetectDomains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/iris-detect/domains/ignored/\n  method: get\n  operationId: getDetectIgnored\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/iris-detect/domains/new/\n  method: get\n  operationId: getDetectNewDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/iris-detect/domains/watched/\n  method: get\n  operationId: getDomainsWatched\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/iris-detect/escalations/\n  method: post\n  operationId: postDetectEscalations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/iris-detect/monitors/\n  method: get\n  operationId: getDetectMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/iris-detect/monitors/\n  method: post\n  operationId: postDetectMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/iris-detect/monitors/\n  method: put\n  operationId: putDetectMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/iris-detect/monitors/\n  method: delete\n  operationId: deleteDetectMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/iris-enrich/\n  method: get\n  operationId: getIrisEnrich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/iris-enrich/\n\
  \  method: post\n  operationId: postIrisEnrich\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/iris-investigate/\n  method: get\n  operationId: getIrisInvestigate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/iris-investigate/\n  method: post\n  operationId: postIrisInvestigate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/\n  method: get\n  operationId: getAccountInfo\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/\n  method: get\n  operationId: getAccountInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{domain}/\n  method: get\n  operationId: getDomainProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{domain}/hosting-history/\n  method: get\n  operationId: getHostingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{domain}/rdap/parsed/\n  method: get\n  operationId: getParsedDomainRdap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/{query}/whois/\n  method: get\n  operationId: getWhoisLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{domain}/whois/history/\n  method: get\n  operationId: getWhoisHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{query}/whois/parsed/\n  method: get\n  operationId: getParsedWhois\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reputation/\n  method: get\n  operationId: getDomainReputation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk/\n  method: get\n  operationId: getDomainRiskScore\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk/evidence/\n  method: get\n  operationId: getRiskScoreEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{ip}/host-domains/\n  method: get\n  operationId: getHostDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{nameServer}/name-server-domains/\n  method: get\n  operationId: getNameServerDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{domain}/reverse-ip/\n  method: get\n  operationId: getReverseIpForDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reverse-ip-whois/\n  method: get\n  operationId: getReverseIpWhois\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reverse-whois/\n  method: get\n  operationId: getReverseWhois\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/domain-search/\n  method: get\n  operationId: getDomainSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domain-history/\n  method: get\n  operationId: getDomainHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ip-monitor/\n  method: get\n  operationId: getIpMonitor\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mark-alert/\n  method: get\n  operationId: getBrandMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/name-server-monitor/\n  method: get\n  operationId: getNameServerMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/registrant-alert/\n  method: get\n  operationId: getRegistrantMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /siebatchd/v1/validate\n  method: post\n  operationId: validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /siebatchd/v1/siebatch/chdetails\n  method: post\n  operationId: chdetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /siebatchd/v1/siebatch/chfetch\n  method: post\n  operationId: chfetch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /siebatchd/v1/siebatch/makeurl\n  method: post\n  operationId: makeurl\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/agentic-access/domaintools-agentic-access.yml
summary_line: 53 operations · 11 acting · 1 human-in-the-loop
tags:
- Company
- Threat Intelligence
- Domain Intelligence
- DNS
- WHOIS
- Passive DNS
- Cybersecurity
- Domain Monitoring
- Risk Scoring
- Security
---
