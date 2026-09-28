---
acting_count: 0
action_class_counts:
  connected: 53
api_specs:
- filename: synthient-account-api-openapi.yml
  format: yaml
  label: Synthient API Account API
  slug: synthient-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-account-api-openapi.yml
- filename: synthient-anonymizers-api-openapi.yml
  format: yaml
  label: Synthient API Anonymizers API
  slug: synthient-anonymizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-anonymizers-api-openapi.yml
- filename: synthient-helios-api-openapi.yml
  format: yaml
  label: Synthient API Helios API
  slug: synthient-helios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-helios-api-openapi.yml
- filename: synthient-ja4t-api-openapi.yml
  format: yaml
  label: Synthient API JA4T API
  slug: synthient-ja4t-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-ja4t-api-openapi.yml
- filename: synthient-lookup-api-openapi.yml
  format: yaml
  label: Synthient API Lookup API
  slug: synthient-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-lookup-api-openapi.yml
- filename: synthient-proxies-api-openapi.yml
  format: yaml
  label: Synthient API Proxies API
  slug: synthient-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-proxies-api-openapi.yml
- filename: synthient-torrents-api-openapi.yml
  format: yaml
  label: Synthient API Torrents API
  slug: synthient-torrents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-torrents-api-openapi.yml
consequence_counts:
  read: 53
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Synthient Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 53
overview: 'Synthient API exposes 53 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 53 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Synthient API
provider_slug: synthient
slug: synthient-agentic-access
source_filename: synthient-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: generated\nsource: openapi/synthient-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 53\n  by_consequence:\n    read: 53\n  human_in_the_loop_required: 0\noperations:\n- path: /account/me\n  method: get\n  operationId: getAccountInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/anonymizers/export\n  method: get\n  operationId: listAnonymizersExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/anonymizers/export/{date}\n  method:\
  \ get\n  operationId: downloadAnonymizersExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/anonymizers/export/{date}/meta\n  method: get\n  operationId: getAnonymizersExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/anonymizers/export/{date}/{hour}\n  method: get\n  operationId: downloadAnonymizersHourlyExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/anonymizers/export/{date}/{hour}/meta\n  method: get\n  operationId: getAnonymizersHourlyExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/anonymizers/stream\n\
  \  method: get\n  operationId: streamAnonymizers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/adb/export\n  method: get\n  operationId: listHoneypotADBExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/adb/export/{date}\n  method: get\n  operationId: downloadHoneypotADBExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/adb/export/{date}/meta\n  method: get\n  operationId: getHoneypotADBExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/adb/export/{date}/{hour}\n  method: get\n  operationId: downloadHoneypotADBHourlyExport\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/adb/export/{date}/{hour}/meta\n  method: get\n  operationId: getHoneypotADBHourlyExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/adb/stream\n  method: get\n  operationId: streamHoneypotADB\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/dns/export\n  method: get\n  operationId: listHoneypotDNSExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/dns/export/{date}\n  method: get\n  operationId: downloadHoneypotDNSExport\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/dns/export/{date}/meta\n  method: get\n  operationId: getHoneypotDNSExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/dns/export/{date}/{hour}\n  method: get\n  operationId: downloadHoneypotDNSHourlyExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/dns/export/{date}/{hour}/meta\n  method: get\n  operationId: getHoneypotDNSHourlyExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/dns/stream\n  method: get\n  operationId: streamHoneypotDNS\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/http/export\n  method: get\n  operationId: listHoneypotHTTPExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/http/export/{date}\n  method: get\n  operationId: downloadHoneypotHTTPExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/http/export/{date}/meta\n  method: get\n  operationId: getHoneypotHTTPExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/http/export/{date}/{hour}\n  method: get\n  operationId: downloadHoneypotHTTPHourlyExport\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/http/export/{date}/{hour}/meta\n  method: get\n  operationId: getHoneypotHTTPHourlyExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/http/stream\n  method: get\n  operationId: streamHoneypotHTTP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/https/export\n  method: get\n  operationId: listHoneypotHTTPSExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/https/export/{date}\n  method: get\n  operationId: downloadHoneypotHTTPSExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/https/export/{date}/meta\n  method: get\n  operationId: getHoneypotHTTPSExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/https/export/{date}/{hour}\n  method: get\n  operationId: downloadHoneypotHTTPSHourlyExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/https/export/{date}/{hour}/meta\n  method: get\n  operationId: getHoneypotHTTPSHourlyExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/helio/https/stream\n  method: get\n  operationId: streamHoneypotHTTPS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/ja4t/export\n  method: get\n  operationId: listJA4TExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/ja4t/export/{date}\n  method: get\n  operationId: downloadJA4TExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/ja4t/export/{date}/meta\n  method: get\n  operationId: getJA4TExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/ja4t/export/{date}/{hour}\n  method: get\n  operationId: downloadJA4THourlyExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/ja4t/export/{date}/{hour}/meta\n\
  \  method: get\n  operationId: getJA4THourlyExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/ja4t/stream\n  method: get\n  operationId: streamJA4T\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/proxies/export\n  method: get\n  operationId: listProxiesExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/proxies/export/{date}\n  method: get\n  operationId: downloadProxiesExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/proxies/export/{date}/meta\n  method: get\n  operationId: getProxiesExportMeta\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/proxies/export/{date}/{hour}\n  method: get\n  operationId: downloadProxiesHourlyExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/proxies/export/{date}/{hour}/meta\n  method: get\n  operationId: getProxiesHourlyExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/proxies/stream\n  method: get\n  operationId: streamProxies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/torrents/export\n  method: get\n  operationId: listTorrentsExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/torrents/export/{date}\n  method: get\n  operationId: downloadTorrentsExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/torrents/export/{date}/meta\n  method: get\n  operationId: getTorrentsExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/torrents/export/{date}/{hour}\n  method: get\n  operationId: downloadTorrentsHourlyExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/torrents/export/{date}/{hour}/meta\n  method: get\n  operationId: getTorrentsHourlyExportMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/torrents/stream\n  method: get\n  operationId: streamTorrents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/domain/{domain}\n  method: get\n  operationId: domainLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/ip/{ip_address}\n  method: get\n  operationId: ipLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/ips\n  method: post\n  operationId: lookupIpBatch\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/agentic-access/synthient-agentic-access.yml
summary_line: 53 operations
tags:
- Company
- IP
- Enrichment
- Cybersecurity
- Data
---
