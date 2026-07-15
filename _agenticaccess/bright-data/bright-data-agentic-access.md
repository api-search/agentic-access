---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 29
api_specs:
- filename: bright-data-web-unlocker-api-openapi.yml
  format: yaml
  label: Bright Data Web Unlocker API
  slug: web-unlocker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-web-unlocker-api-openapi.yml
- filename: bright-data-serp-api-openapi.yml
  format: yaml
  label: Bright Data SERP API
  slug: serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-serp-api-openapi.yml
- filename: bright-data-web-scraper-api-openapi.yml
  format: yaml
  label: Bright Data Web Scraper API
  slug: web-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-web-scraper-api-openapi.yml
- filename: bright-data-scraping-browser-api-openapi.yml
  format: yaml
  label: Bright Data Scraping Browser API
  slug: scraping-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-scraping-browser-api-openapi.yml
- filename: bright-data-deep-lookup-api-openapi.yml
  format: yaml
  label: Bright Data Deep Lookup API
  slug: deep-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-deep-lookup-api-openapi.yml
- filename: bright-data-web-archive-api-openapi.yml
  format: yaml
  label: Bright Data Web Archive API
  slug: web-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-web-archive-api-openapi.yml
- filename: bright-data-dataset-marketplace-api-openapi.yml
  format: yaml
  label: Bright Data Dataset Marketplace API
  slug: dataset-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-dataset-marketplace-api-openapi.yml
- filename: bright-data-account-management-api-openapi.yml
  format: yaml
  label: Bright Data Account Management API
  slug: account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-account-management-api-openapi.yml
- filename: bright-data-proxy-manager-api-openapi.yml
  format: yaml
  label: Bright Data Proxy Manager API
  slug: proxy-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-proxy-manager-api-openapi.yml
- filename: bright-data-scraping-shield-api-openapi.yml
  format: yaml
  label: Bright Data Scraping Shield API
  slug: scraping-shield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-scraping-shield-api-openapi.yml
consequence_counts:
  physical: 1
  read: 29
  safety-critical: 1
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Bright Data Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /zone/change_disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/refresh_ips
operation_count: 56
overview: 'Bright Data exposes 56 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 25 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bright Data
provider_slug: bright-data
slug: bright-data-agentic-access
source_filename: bright-data-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bright-data-account-management-api-openapi.yml, openapi/bright-data-dataset-marketplace-api-openapi.yml,\n  openapi/bright-data-deep-lookup-api-openapi.yml, openapi/bright-data-proxy-manager-api-openapi.yml,\n  openapi/bright-data-scraping-browser-api-openapi.yml, openapi/bright-data-scraping-shield-api-openapi.yml,\n  openapi/bright-data-serp-api-openapi.yml, openapi/bright-data-web-archive-api-openapi.yml,\n  openapi/bright-data-web-scraper-api-openapi.yml, openapi/bright-data-web-unlocker-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    acting: 27\n    connected: 29\n  by_consequence:\n    write: 25\n    read: 29\n    safety-critical: 1\n\
  \    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /zone\n  method: post\n  operationId: addZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zone\n  method: get\n  operationId: getZone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zone\n  method: delete\n  operationId: deleteZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zone/change_disable\n  method: post\n  operationId: toggleZone\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /zone/ips\n  method: get\n  operationId: listZoneIps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zone/ips\n  method: post\n  operationId: addZoneIps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zone/ips\n  method: delete\n  operationId: removeZoneIps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zone/ips/refresh\n  method: post\n  operationId: refreshZoneIps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zone/whitelist\n  method: post\n  operationId: addWhitelist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zone/blacklist\n  method: post\n  operationId: addBlacklist\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zone/domain_perm\n  method: get\n  operationId: getDomainPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/balance\n  method: get\n  operationId: getCustomerBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zone/bw\n  method: get\n  operationId: getZoneBandwidth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: get\n  operationId: listMarketplaceDatasets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/metadata\n  method: get\n  operationId: getDatasetMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/snapshots/{snapshot_id}\n  method: get\n  operationId: getDatasetSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/snapshots/{snapshot_id}/deliver\n  method: post\n  operationId: deliverDatasetSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deep_lookup/trigger\n\
  \  method: post\n  operationId: triggerDeepLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deep_lookup/preview\n  method: post\n  operationId: previewDeepLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deep_lookup/enhance_query\n  method: post\n  operationId: enhanceDeepLookupQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /deep_lookup/request/{request_id}/status\n  method: get\n  operationId: getDeepLookupStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deep_lookup/request/{request_id}/download\n  method: get\n  operationId: downloadDeepLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deep_lookup/request/{request_id}/enrich\n  method: post\n  operationId: enrichDeepLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/proxies\n  method: get\n  operationId: listProxies\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/proxies\n  method: post\n  operationId: createProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/proxies/{port}\n  method: get\n  operationId: getProxy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/proxies/{port}\n  method: put\n  operationId: updateProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/proxies/{port}\n  method: delete\n  operationId: deleteProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/proxies/{port}/banip\n  method: post\n  operationId: banIp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/refresh_ips\n  method: post\n  operationId: refreshIps\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/zones\n  method: get\n  operationId: listZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gen_token\n  method: get\n  operationId: genToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /browser_sessions\n  method: get\n  operationId: listBrowserSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /browser_sessions/{session_id}\n  method: get\n  operationId: getBrowserSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /shield/class\n  method: get\n  operationId: listShieldClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shield/domains_by_class\n  method: get\n  operationId: domainsByClass\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shield/samples\n  method: get\n  operationId: getShieldSamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shield/zones_by_class\n  method: get\n  operationId: zonesByClass\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serp/req\n  method: post\n  operationId: submitSerpRequest\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serp/get_result\n  method: get\n  operationId: getSerpResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webarchive/search\n  method: post\n  operationId: submitArchiveSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webarchive/search/{search_id}\n  method: get\n  operationId: getArchiveSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /webarchive/searches\n  method: get\n  operationId: listArchiveSearches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webarchive/deliver-to-cloud\n  method: post\n  operationId: deliverArchiveToCloud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/v3/scrape\n  method: post\n  operationId: triggerScrape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /datasets/v3/progress/{snapshot_id}\n  method: get\n  operationId: getScrapeProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/v3/log/{snapshot_id}\n  method: get\n  operationId: getSnapshotLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/v3/snapshots\n  method: get\n  operationId: listSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/v3/snapshot/{snapshot_id}/cancel\n  method: post\n  operationId: cancelSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/v3/snapshot/{snapshot_id}/rerun\n  method: post\n  operationId: rerunSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/v3/snapshot/{snapshot_id}\n  method: get\n  operationId: downloadSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/v3/snapshot/{snapshot_id}/deliver\n  method: post\n  operationId: deliverSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /request\n  method: post\n  operationId: unlockSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unblocker/req\n  method: post\n  operationId: unlockAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unblocker/get_result\n  method: get\n \
  \ operationId: getUnlockResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/agentic-access/bright-data-agentic-access.yml
summary_line: 56 operations · 27 acting · 1 human-in-the-loop
tags:
- Web Data
- Web Scraping
- Proxy
- Residential Proxy
- Datacenter Proxy
- ISP Proxy
- Mobile Proxy
- SERP
- Web Unlocker
- Scraping Browser
- Dataset Marketplace
- MCP
- AI Agents
---
