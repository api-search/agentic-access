---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 39
api_specs:
- filename: shodan-rest-openapi.yml
  format: yaml
  label: Shodan REST API
  slug: shodan-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-rest-openapi.yml
- filename: shodan-stream-openapi.yml
  format: yaml
  label: Shodan Streaming API
  slug: shodan-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-stream-openapi.yml
- filename: shodan-trends-openapi.yml
  format: yaml
  label: Shodan Trends API
  slug: shodan-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-trends-openapi.yml
- filename: shodan-internetdb-openapi.yml
  format: yaml
  label: InternetDB API
  slug: internetdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-internetdb-openapi.yml
- filename: shodan-cvedb-openapi.yml
  format: yaml
  label: CVEDB API
  slug: cvedb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-cvedb-openapi.yml
consequence_counts:
  read: 39
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Shodan Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /shodan/alert/{id}/trigger/{trigger}
operation_count: 51
overview: 'Shodan exposes 51 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 39 read, 11 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shodan
provider_slug: shodan
slug: shodan-agentic-access
source_filename: shodan-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/shodan-cvedb-openapi.yml, openapi/shodan-internetdb-openapi.yml, openapi/shodan-rest-openapi.yml,\n  openapi/shodan-stream-openapi.yml, openapi/shodan-trends-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    connected: 39\n    acting: 12\n  by_consequence:\n    read: 39\n    write: 11\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /cve/{cveId}\n  method: get\n  operationId: getCve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cves\n  method: get\n  operationId: searchCves\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpes\n  method: get\n  operationId: searchCpes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}\n  method: get\n  operationId: getInternetDbHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/host/{ip}\n  method: get\n  operationId: getHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/host/count\n  method: get\n  operationId: getHostCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/host/search\n  method: get\n  operationId:\
  \ searchHosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/host/search/facets\n  method: get\n  operationId: listSearchFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/host/search/filters\n  method: get\n  operationId: listSearchFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/host/search/tokens\n  method: get\n  operationId: tokenizeSearchQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/ports\n  method: get\n  operationId: listPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/protocols\n  method: get\n  operationId: listProtocols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/scan\n  method: post\n  operationId: createScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shodan/scan/internet\n  method: post\n  operationId: createInternetScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shodan/scans\n\
  \  method: get\n  operationId: listScans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/scan/{id}\n  method: get\n  operationId: getScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/alert\n  method: post\n  operationId: createAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shodan/alert/info\n  method: get\n  operationId: listAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/alert/{id}/info\n  method:\
  \ get\n  operationId: getAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/alert/{id}\n  method: post\n  operationId: updateAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shodan/alert/{id}\n  method: delete\n  operationId: deleteAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shodan/alert/triggers\n  method: get\n  operationId: listAlertTriggers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/alert/{id}/trigger/{trigger}\n  method: put\n  operationId: enableAlertTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shodan/alert/{id}/trigger/{trigger}\n  method: delete\n  operationId: disableAlertTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /notifier\n  method: get\n  operationId: listNotifiers\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifier\n  method: post\n  operationId: createNotifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifier/provider\n  method: get\n  operationId: listNotifierProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifier/{id}\n  method: get\n  operationId: getNotifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifier/{id}\n  method: put\n  operationId: updateNotifier\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifier/{id}\n  method: delete\n  operationId: deleteNotifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shodan/query\n  method: get\n  operationId: listSavedQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/query/search\n  method: get\n  operationId: searchSavedQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /shodan/query/tags\n  method: get\n  operationId: listSavedQueryTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/data\n  method: get\n  operationId: listBulkDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/data/{dataset}\n  method: get\n  operationId: listBulkDatasetFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/domain/{domain}\n  method: get\n  operationId: getDomainDns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/resolve\n  method: get\n  operationId: resolveHostnames\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/reverse\n  method: get\n  operationId: reverseDnsLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/httpheaders\n  method: get\n  operationId: getHttpHeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/myip\n  method: get\n  operationId: getMyIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/profile\n  method: get\n  operationId: getAccountProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-info\n\
  \  method: get\n  operationId: getApiInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/member/{user}\n  method: put\n  operationId: addOrganizationMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/member/{user}\n  method: delete\n  operationId: removeOrganizationMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shodan/banners\n  method: get\n  operationId: streamBanners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/asn/{asn}\n  method: get\n  operationId: streamBannersByAsn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/countries/{countries}\n  method: get\n  operationId: streamBannersByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shodan/ports/{ports}\n  method: get\n  operationId: streamBannersByPort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /shodan/vulns/{vulns}\n  method: get\n  operationId: streamBannersByVuln\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  operationId: searchTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/agentic-access/shodan-agentic-access.yml
summary_line: 51 operations · 12 acting · 1 human-in-the-loop
tags:
- Security
- Search
- Internet
- Devices
- IoT
- Vulnerabilities
- CVE
- Attack Surface
- Threat Intelligence
- Reconnaissance
- Network
- DNS
- Scanning
- Public APIs
---
